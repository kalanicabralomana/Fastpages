---
toc: true
layout: post
description: Binary usage
categories: [markdown, Final]
title: Binary usage
---

<div class="container bg-primary">
    <form>
        <div class="form-group row">
            Type a decimal number and press tab to convert to binary:
            <div>
                <input onblur="convert()" type="text" name="decimal" id="decimal"/><br>
            </div>
        </div>
        <div class="form-group row">
            Binary : <span id="binary" ></span>
        </div>
    </form>
</div>

<script>
    function convert(){
        var array = document.getElementsByName('decimal');  // user input (can be letters, symbols, etc. (strings))
        if (array[array.length-1].value.length != 0) {  // skip the process if user input is literally nothing 
            var binary = [];  // stores binary result
            var decimal = parseInt(array[0].value)  // user decimal input
            var rem;  // temporary variable to store remainder
            if (decimal == "0") {  // if user input is decimal 0, binary output will also be 0
                binary.unshift("0");
            }
            else {
                while (decimal != 0){  // continues until quotient becomes 0  
                    rem = decimal%2;  // %2 calculates the remainder of given decimal
                    binary.unshift(rem);  // stores remainder 
                    decimal = Math.floor(decimal/2)  // rounds down decimal / 2
                }
            } 
            const final = binary.join('');  // converts array to string (for example, array may be 1,0,1,0,0 and a string is 10100)
            document.getElementById('binary').innerHTML = final;   // sends binary to html
        }
        // moves the curser on textbox 
        document.getElementById("decimal").focus();
    }

</script>