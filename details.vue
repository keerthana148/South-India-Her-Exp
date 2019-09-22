<template>
    <div class="Fill the details>
    <p>
        <script type="text/javascript" src="http://code.jquery.com/jquery-1.8.2.js"></script>
        <script type="text/javascript" src="http://code.jquery.com/ui/1.10.3/jquery-ui.js"></script>
    </p>
        <script type="text/javascript">
            $(function(){
                $("onclick").click(function(){
                $("divpopup").dialog({
                    title:"Confirm",
                    width: 430,''
                    height:200,
                    modal:true,
                    buttons:{
                        confirm:
                            function(){
                                $(this).dialog('Confirm Booking');
                            }
                    }
                });
                });
            })
        </script>

        <div class="container">
            <form>
                <p class="paragraph"> Please fill the details</p>
                <input type="text" name="firstname" placeholder="First Name" class="ipt"/>
                <input type="text" name="lastname" placeholder="Last Name" class="ipt"/>
                <br>
                <input type="text" name="email" placeholder="Email Id" class="ipt"/>
                <input type="text" name="phone no" placeholder="Contact No" class="ipt"/>
                <br>
                <textarea name="address" placeholder="Address" class="area" row="5" required></textarea>
                <select class="selection">
                    <option>Select the Govt Id</option>
                    <option value="adhar card">Adhar card</option>
                    <option value="pan card">PAN card</option>
                    <option value="voter id">Voter Id</option>
                </select>
                <br>
                <input type="text" name="adults" placeholder="Enter no of adults" class="ipt"/>
                <input type="text" name="children" placeholder="Enter no of children" class="ipt"/>
                <br>
                <input type="text" name="no of seats" placeholder="Total seats" class="ipt"/>
                <select class="selection">
                    <option>Select the Coach</option>
                    <option value="cc">Club Class</option>
                    <option vlaue="pc">Premier Class</option>
                    <option value="ec">Executive Class</option>
                </select>
                <br>
                //total amount
                <div id="divpopup" sytle="display:none">
                    Please confirm your tickets
                </div>
                <button type="button" id="btnclick" title="Book now"></button>
                
            </form>
        </div>
    </div>
</template>

<style scoped>
body
{
    background-color: #ccc;
    padding: 0px;
    margin: 0px;

}
.container
{
    background: #fff;
    width: 700px;
    height: 900px;
    border-radius: 03px;
    margin: 0 auto;
    border-bottom: 1px solid #ccc;
    margin-top:50px;
}
.paragraph
{
    background-color: #2980b9;
    color: white;
    font-family: sans-serif;
    text-align: center;
    border-radius: 03px;
    padding: 15px 0px 15px 0px;
    margin-bottom: 50px;
}
.ipt
{
    width: 225px;
    height: 35px;
    border-radius: 02px;
    border: none;
    border: 1px;
    margin-left: 25px;
    padding-left: 05px;
    border-left: 03px solid #27ae60;
    margin-top: 10px;
}
.area
{
    width: 225px;
    height: 70px;
    border-radius: 02px;
    border: none;
    border: 1px;
    margin-left: 25px;
    padding-left: 05px;
    border-left: 03px solid #27ae60;
    margin-top: 10px; 
}
.selection
{
    width: 225px;
    height: 30px;
    font-family: sans-serif;
    margin-left: 25px;
}
</style>

