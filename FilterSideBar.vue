<template>
    <div>
  <div class="d-flex justify-content-center"> 
    <div class="wrapper center-block"> 
        <div class="filters-text"> 
            <span class="filter-span">Filters <small>(find product using filters below)</small></span>
            <span style="float:right;"><i class="fa fa-filter"></i></span>
        </div>  
        <div class="panel-group" id="accordion" role="tablist" aria-multiselectable="true">
            <div class="panel panel-default">
                <div class="panel-heading" role="tab" id="heading1">  
                    <h4 class="panel-title"> <a class="collapsed" role="button" data-toggle="collapse" data-parent="#accordion" href="#collapse1" aria-expanded="false" aria-controls="collapse1"> Processors </a> </h4>
                </div> 
                <div id="collapse1" class="panel-collapse collapse" role="tabpanel" aria-labelledby="heading1">
                    <div class="panel-body">
                        <div class="checkbox"> <label> <input type="checkbox" class="option-input checkbox" name="filter[]" value="12" /> <span class="ml-10">CORE i5</span> </label> </div>
                        <div class="checkbox"> <label> <input type="checkbox" class="option-input checkbox" name="filter[]" value="12" /> <span class="ml-10">CORE i7</span> </label> </div>
                    </div>
                </div>
            </div>
            <div class="panel panel-default">
                <div class="panel-heading" role="tab" id="heading2">
                    <h4 class="panel-title"> <a class="collapsed" role="button" data-toggle="collapse" data-parent="#accordion" href="#collapse2" aria-expanded="false" aria-controls="collapse2"> Brand </a> </h4>
                </div>
                <div id="collapse2" class="panel-collapse collapse" role="tabpanel" aria-labelledby="heading2">
                    <div class="panel-body">
                        <div class="checkbox"> <label> <input type="checkbox" class="option-input checkbox" name="filter[]" value="12" /> <span class="ml-10">APPLE</span> </label> </div>
                        <div class="checkbox"> <label> <input type="checkbox" class="option-input checkbox" name="filter[]" value="12" /> <span class="ml-10">DELL</span> </label> </div>
                        <div class="checkbox"> <label> <input type="checkbox" class="option-input checkbox" name="filter[]" value="12" /> <span class="ml-10">HP</span> </label> </div>
                    </div>
                </div>
            </div>
            <div class="panel panel-default">
                <div class="panel-heading" role="tab" id="heading3">
                    <h4 class="panel-title"> <a class="collapsed" role="button" data-toggle="collapse" data-parent="#accordion" href="#collapse3" aria-expanded="false" aria-controls="collapse3"> Screen Size </a> </h4>
                </div>
                <div id="collapse3" class="panel-collapse collapse" role="tabpanel" aria-labelledby="heading3">
                    <div class="panel-body"> 
                        <div class="checkbox"> <label> <input type="checkbox" class="option-input checkbox" name="filter[]" value="12" /> <span class="ml-10">BELOW 12.9 INCH</span> </label> </div>
                        <div class="checkbox"> <label> <input type="checkbox" class="option-input checkbox" name="filter[]" value="12" /> <span class="ml-10">12 INCH - 12.9 INCH</span> </label> </div>
                        <div class="checkbox"> <label> <input type="checkbox" class="option-input checkbox" name="filter[]" value="12" /> <span class="ml-10">13 INCH - 13.9 INCH</span> </label> </div>
                    </div>
                </div> 
            </div>
            <div class="panel panel-default">
                <div class="panel-heading" role="tab" id="heading4">
                    <h4 class="panel-title"> <a class="collapsed" role="button" data-toggle="collapse" data-parent="#accordion" href="#collapse4" aria-expanded="false" aria-controls="collapse4"> Operating System </a> </h4>
                </div>
                <div id="collapse4" class="panel-collapse collapse" role="tabpanel" aria-labelledby="heading4">
                    <div class="panel-body">
                        <div class="checkbox"> <label> <input type="checkbox" class="option-input checkbox" name="filter[]" value="12" /> <span class="ml-10">Windows 7</span> </label> </div>
                        <div class="checkbox"> <label> <input type="checkbox" class="option-input checkbox" name="filter[]" value="12" /> <span class="ml-10">windows 8</span> </label> </div>
                        <div class="checkbox"> <label> <input type="checkbox" class="option-input checkbox" name="filter[]" value="12" /> <span class="ml-10">Windows 10</span> </label> </div>
                        <div class="checkbox"> <label> <input type="checkbox" class="option-input checkbox" name="filter[]" value="12" /> <span class="ml-10">MAC OS</span> </label> </div>
                    </div>
                </div>
            </div> 
        </div> 
        <div class="text-right refine"> <button class="btn btn-out btn-primary btn-square" id="button-filter">Refine Search</button> </div>
    </div>
</div>
</div> 
</template>


<style scoped>
  body {
    background-color: #f5f6f7
}

.wrapper {
    width: 30%;
    margin-top: 50px
}

@media(max-width:992px) {
    .wrapper {
        width: 100%
    }
} 
 
.panel-heading {
    padding: 0;
    border: 0;
    padding: 9px 3px !important
}

.panel-title>a,
.panel-title>a:active {
    display: block;
    padding: 10px;
    color: #555;
    font-size: 11px;
    text-transform: uppercase;
    letter-spacing: 1px;
    word-spacing: 3px;
    text-decoration: none
}

.panel-heading a:before {
    font-family: 'Glyphicons Halflings';
    content: "\e114";
    float: right;
    transition: all 0.5s
}

.panel-heading.active a:before {
    -webkit-transform: rotate(180deg);
    -moz-transform: rotate(180deg);
    transform: rotate(180deg)
}

.panel-default>.panel-heading {
    color: #282b2f;
    background-color: #ffffff !important;
    border-color: #d5d5d5
}

@keyframes click-wave {
    0% {
        height: 40px;
        width: 40px;
        opacity: 0.15;
        position: relative
    }

    100% {
        height: 200px;
        width: 200px;
        margin-left: -80px;
        margin-top: -80px;
        opacity: 0
    }
}

.option-input {
    -webkit-appearance: none;
    -moz-appearance: none;
    -ms-appearance: none;
    -o-appearance: none;
    appearance: none;
    position: relative;
    top: -8.66667px;
    right: 0;
    bottom: 0;
    left: 0;
    height: 24px;
    width: 24px;
    transition: all 0.15s ease-out 0s;
    background: #cbd1d8;
    border: none;
    color: #fff;
    cursor: pointer;
    display: inline-block;
    margin-right: 0.5rem;
    outline: none;
    position: relative;
    z-index: 1000
}

.option-input:hover {
    background: #9faab7
}

.option-input:checked {
    background: #2874ef
}

.option-input:checked::before {
    height: 24px;
    width: 24px;
    position: absolute;
    content: "\f111";
    font-family: "Font Awesome 5 Free";
    display: inline-block;
    font-size: 14.66667px;
    text-align: center;
    line-height: 26px
}

.option-input:checked::after {
    -webkit-animation: click-wave 0.15s;
    -moz-animation: click-wave 0.15s;
    animation: click-wave 0.15s;
    background: #E91E63;
    content: '';
    display: block;
    position: relative;
    z-index: 100
}

.option-input.radio {
    border-radius: 50%
}

.option-input.radio::after {
    border-radius: 50%
}

.checkbox input[type="checkbox"],
.checkbox-inline input[type="checkbox"] {
    float: left;
    margin-left: -4px !important;
    margin-top: 9px
}

input[type="checkbox"]:focus {
    outline: thin dotted #333;
    outline: 0px auto -webkit-focus-ring-color;
    outline-offset: 0px
}

.ml-10 {
    margin-left: 10px;
    font-size: 12px;
    color: #080808
}

.btn.btn-out {
    outline: 1px solid #fff;
    outline-offset: -5px
}

.btn {
    border-radius: 2px;
    text-transform: capitalize;
    font-size: 11px;
    padding: 10px 19px;
    cursor: pointer;
    color: #fff
}

.fa {
    font-size: 12px;
    color: #2874ef
}

.refine {
    padding: 0px 0px !important
}

.filters-text {
    background: #fff;
    border: 1px solid #d5d5d5;
    margin-bottom: 15px;
    padding: 12px
}

.filter-span {
    font-size: 17px;
    color: #2874ef
}
</style>
