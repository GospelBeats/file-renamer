# file-renamer
Remove spaces from a file name
Deployed site: https://gospelbeats.github.io/file-renamer/

## Technology Used
- Javascript
- Jquery


### Styling
- Bootstrap

-----------------------------------------------------------------------------------------

![APP Sreenshot](https://github.com/GospelBeats/file-renamer/blob/master/file-renamer.JPG)

-----------------------------------------------------------------------------------------


## Code

`$(document).ready(function(){

  $("button").click(function(){
   
        let fileName = $("#fileName").val();

        if (fileName === "") {
            alert("Please Enter A File Name");
            $("#fileName").val("");
        } else {

        $("#fileName").val("");
        convertString(fileName);

        function convertString(str){

        let option = $( "#opt option:selected" ).text();

        let newStr = str.replace(/ /g, option);

        $("#convertFileName").val(newStr);

            } // if statement

        } // convert string

  }); // button click

}); // document ready`
      

