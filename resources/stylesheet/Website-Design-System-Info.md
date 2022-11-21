# Website-Design-System-Info


**PORIADNE VSETKO OKOMENTOVAT!!!**

**UPRAVIT STRANKU AJ PRE MOBILY - RESPONSIVE DESIGN**

**PRIDAT TLACITKA**

**PRIDAT ESTE JEDNU NAVIGACIU - BREADCRUMB - TAK ZE KAZDA CAST BUDE MAT VLASTNU STRANKU**

**ADD FOOTER****

**Pridaj sekciu na gridy**

********************************************************
INSPIRATION:

https://material.io/design -> **Google`s Material Design**
https://getbootstrap.com/ -> **Twitter Bootstrap**
https://www.lightningdesignsystem.com/utilities/text/ -> **Lighting Design System**

https://discuss.codecademy.com/t/build-a-website-style-guide-challenge-project-html-css/462395?_gl=1*5waslo*_ga*OTgzOTY0MjUzLjE2NjM0MzIwODE.*_ga_3LRZM6TM9L*MTY2NDM4Mjk1Mi4zOS4xLjE2NjQzODI5ODYuMjYuMC4w -> **Projekty ostatnych**

https://www.codecademy.com/journeys/full-stack-engineer/paths/fscj-22-web-development-foundations/tracks/fscj-22-improved-styling-with-css/modules/wdcp-22-build-a-website-design-system-2a08b912-678e-4186-ab57-86a0fb0ca601/projects/independent-project-web-design-system -> **ORIGINAL CODECADEMY PROJECT PAGE**


*********************************************************************

*! Great Flex Tutorial -> https://www.youtube.com/watch?v=u044iM9xsWU&ab_channel=KevinPowell

**********************************************************************

One of the way how to select DIRECT CHILDREN is to use .parent > *

For Example:
    <div class="main-div">
        <div class="direct-child>
        </div>
    </div>

    .main-div > * {

    }

    This would actually select .direct-child

***************************************************************************
**************************************************************************

In order to space items evenly I can use with flex:

    -   justify-content: space-evenly
    -   justify-content: space-between

This take any left over space and distribute it evenly between all of the elements. This is great for **NAVIGATIONS**

This is always implemented in PARENT! .... So for example in <ul> and it will space its children <li> evenly across the parrent <ul>

*****************************************************************

In order to center content verticaly i can use align-items:center . But It will only work when there are for example 2 items and one is bigger so the actual height of div will be the height of the larger one and the left the smaller one will be centered. Id the will be the same height, there will be no extra space to distribute and nothing would happen

************

Let`s consider this case:

<div class="collumns">
    <article class="card">Some random text</article>
    <article class="card">Some random random text</article>
    <article class="card">Some random random random text</article>
</div>

1. When I want to select lets say the second article with class="card" I can do this:

        .card:nth-child(2){
            backround:pink;
            align-self: flex-start;    /* of course there is flex-end, flex-strech*/
        }

And what this does, it lets the children override the parent and therefore any rules form the parent div(regarding flex) are no longer valid and the child can do "its own thing"

Very Very Useful!

