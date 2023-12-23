<template>
    <div class="point" :style="getStyle"></div>
</template>

<script>
export default {
    props: ['width', 'left', 'right', 'top', 'background_color'],
    computed: {
        getStyle(){
            return "width: "+this.width+"px; height: "+this.width+ "px; top:"+this.top+"px; left:"+this.left+"px; right:"+this.right+"px; background-color:"+this.background_color;
        }
    }
}
</script>

<style scoped>
.point {
    position: absolute;
    border-radius: 100%;
    height: 0;
    filter: blur(155px);
    opacity: 0.2;
    
    z-index: -1;
}
</style>