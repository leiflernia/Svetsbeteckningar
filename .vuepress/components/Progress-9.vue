
<template>
    <div>
       <div class="progress">
           <div class="determinate" style="width: 47%;"></div>
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
.progress .indeterminate {
 background-color:#337ab7
}
.progress .indeterminate:before {
 -webkit-animation:indeterminate 2.1s cubic-bezier(.65,.815,.735,.395) infinite;
 animation:indeterminate 2.1s cubic-bezier(.65,.815,.735,.395) infinite
}
.progress .indeterminate:after,.progress .indeterminate:before {
 content:"";
 position:absolute;
 background-color:inherit;
 top:0;
 left:0;
 bottom:0;
 will-change:left,right
}
.progress .indeterminate:after {
 -webkit-animation:indeterminate-short 2.1s cubic-bezier(.165,.84,.44,1) infinite;
 animation:indeterminate-short 2.1s cubic-bezier(.165,.84,.44,1) infinite;
 -webkit-animation-delay:1.15s;
 animation-delay:1.15s
}
</style>