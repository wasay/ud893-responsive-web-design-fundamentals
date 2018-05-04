1 device independent pixel may not be same as 1 hardware pixel

<meta name="viewport" content="width=device-width, initial-scale=1.0">


**************************

for best touch experience, have the object width and height set to 48 pixels

48x48 will be a good click option

at least have 40 pixel tap target to avoid tap issues


<style>
a, button, input[type=button], input[type=submit]
{
	min-width:48px;
	min-height:48px;
}

/* OR */

a, button, input[type=button], input[type=submit]
{
	padding: 1.5em;
}
</style>
**************************

start from small form factor to large form factors

mobile first, tablet, and laptops and desktops

it's better to go from small to large as it helps in prioritize the content

header and nav, set width to 100%

make sure of full viewport by using 100% width


320 pixels, could be the smallest device width

**************************
<img id="owl">
#owl {
    width: 640px;
    max-width: 100%;
}

<img class="logo">
.logo {
    width: 125px;
}

<div class="city"></div>
.city{
    width: 100%;
}
**************************

<link rel="stylesheet" href="styles.css">

// stay with SCREEN OR PRINT
// ALL OTHER MEDIA QUERIES ARE NOT MUCH IN USE

<link rel="stylesheet" media="screen and (min-width: 500px)"
    href="over500.css" >

OR

<style>
    @media screen and (min-width: 500px) {
        /* */
    }
</style>

OR

// IMPORT TAGS are not good for performace
<style>
    @import url("over500.css" only screen and (min-width: 500px);
</style>

**************************
Media Queries
**************************

                    scan

mm-aspect-ratio     aspect          max-aspect-ratio
min-color           color           max-color
min-height          height          max-height
min-width           width           max-width
min-resolution      resolution      max-resolution

                    grid


// AVOID
min-device-width    max-device-width
**************************


// style
.container {
    display: flex;
    flex-wrap: wrap;
}
.box {
    height: 100px;
    text-align: center;
    width: 100%;
}