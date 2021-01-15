
<template>
    <div>
       <div class="progress">
           <div class="determinate" style="width: 37%;"></div>
        </div>
    </div>
</template>



<style scoped>
.progress {
 position:relative;
 height:4px;
 display:block;
 width:100%;
 /* background-color:#c0dcdf; */
 border-radius:2px;
 margin:.5rem 0 1rem 0;
 overflow:hidden
}
.progress .determinate {
 position:absolute;
 top:0;
 left:0;
 bottom:0;
 background-color:#14a3af;
 -webkit-transition:width .3s linear;
 transition:width .3s linear
}

</style>