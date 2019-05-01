# css-positioning

// BOX-MODEL applies on block level elements(display: block) not inline-elements, padding and border apllies on inline elemnets but margin and width doesn't work to make it work we have to add display block/inline-block property, by default inline-block looks like inline

//Block Level Elements - <p>,<div>
//Inline Level Elements - <a>,<span>

//FLOAT makes element out of the normal document flow within the container and set it positioned as per the value
clear: both/left/right -- to use in the element when it is float with floated elments to make it work like normal document flow still it doesn't work properly as it starts beneath it but margin doesnt work to make it work we have to use <div style="clear: both;"></div>(it's not a good practice as it is adding unnecessary div to the dom) --- div:after{content: "",display:block;clear: both;}

paragraph into columns
p {
    -webkit-column-count: 3;
    column-count: 3;
    -webkit-column-gap: 50px;
    column-gap: 50px;
    -webkit-column-rule: 1px solid #ccc;
    column-rule: 1px solid #ccc;
    text-align: justify;
}

position: absolute is always relative to the parent which is having relative position whereas fixed always positioned itself to document window

stacking order matter that's why fixed element put at the bottom else overridden by below elemnets while scrolling, z-index will solve the issue

when content clipped out of the container using overflow we can add scroll or make it fit within the container
