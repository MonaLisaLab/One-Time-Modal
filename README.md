# One-Time-Modal

<img width="720" alt="スクリーンショット 2022-07-13 13 45 33" src="https://user-images.githubusercontent.com/83240059/178652625-e08af64d-2435-4567-ad98-008c118e7477.png">

Micro-library for displaying a modal only once.<br>

Use this to display updates and tutorials only once in a hybrid app, or to announce a campaign on a website only once.<br>
Users cannot scroll the background while the modal is displayed.<br><br>

👉<a href="https://toshihidemiyake.github.io/One-Time-Modal-Demo/">DEMO</a>

# Usage

Prepare a container and a modal.
````html

<div class="OTmodal-wrapper">
  <div class="onetimemodal">
  
  </div>
</div>

````

Show a modal
````js
OneTimeModal()
````

Close a modal
````js
CloseModal()
````

Reset the key and allow the modal to be displayed again. Use for testing.
````js
KeyReset()
````

The modal and container styles are set as follows. Feel free to edit them if you don't like.
````js
// You can change modal's style here
const modalwrapper="position:fixed; top:0%; left:0%;"+
                  "width:100vw;"+
                  "height:100vh;"+
                  "z-index:10;"+
                  "display:none;"+
                  "justify-content:center; align-items:center;"+
                  "background-color:inherit;"

const modalcss="display:flex;"+ 
               "justify-content:center; align-items:center; flex-direction:column; gap:50px;"+ 
               "font-size:1em;"+ 
               "background-color:rgb(241, 245, 249);"+ 
               "color:rgb(72, 72, 72);"+ 
               "max-width:90vw;"+
               "padding:50px;"+
               "max-height:80vh;" +
               "border-radius:20px;"
````
