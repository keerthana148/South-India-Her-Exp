<template>
    <div class="Payment page">
        <script type="text/javascript">
            var mywindow;
            function openpopup()
            {
                mywi
            }
        </script>

        <div class="app-container">
            <div class="top-box">
                <p><span class="left-icon">&#x2190;</span>CHECKOUT<span class="right-icon">&#xb7;&#xb7;&#xb7;</span></p>
            </div>
            <div class="middle-box">
                <h1>//need to add total amount<span>Rupees</span></h1>
                <p>Pay to South Indian Heritage Express</p>
            </div> 
            <div class="bottom-box">
                <button type="button" class="payment-option-btn">Pay using Google pay</button>
                <button type="button" class="payment-option-btn">Pay using Net Banking</button>
            
                <div class="card-details">
                <p>Pay using credit or debit card</p>
                <div class="card-num-feild-group">
                <label>Card Number</label><br>
                <input type="text" class="card-num-field" placeholder="xxxx-xxxx-xxxx">
                </div>
                <div class="date-feild-group">
                <label>Expiry Date</label><br>
                <input type="text" class="date-feild" placeholder="mm">
                <input type="text" class="date-feild" placeholder="yyyy">
                </div>
                <div class="cvv-feild-group">
                <label>CVV</label><br>
                <input type="password" class="cvv-feild" placeholder="xxx">
                </div>
                <div class="name-feild-group">
                <label>Card Holder Name</label><br>
                <input type="text" class="name-feild" placeholder="Full Name">
                </div>
                <a  onclick="pop()" class="btn">Pay Now</a>
                <div id="box">
                    <span class="icon-checkmark-round">
                        <h1>You have successfully booked the tickets <a href="ticket.vue">Click Here</a> to download or to view the ticket</h1>
                        <a  onclick="pop()" class="close">Close</a>
                    </span>
                </div>
                <script type="text/javascript">
                    var c =0;
                    function pop(){
                        if(c==0){
                            document.getElementById('box').style.display="block";
                            c=1;
                        }else{
                            document.getElementById('box').style.display="none";
                            c=090;   
                        }
                    }
                    
                </script>

            </div>
        </div>
    </div>
</template>

<style scoped>
*
{
    margin: 0;
    padding: 0;
}
body
{
    font-family: sans-serif;
}
.app-container
{
    height: 600px;
    width: 350px;
    background-image: linear-gradient(#580e8f,#9200ff);
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
    position: absolute;
}
.top-box
{
    height: 150px;
    background-color: #9100fb;
    border-bottom-left-radius: 80px;
    border-bottom-right-radius: 80px;
}
.top-box p
{
    text-align: center;
    padding-top: 20px;
    color: #fff;
}
.left-icon
{
    float: left;
    margin-left: 30px;
}
.middle-box
{
    height: 150px;
    background-image: linear-gradient(#580e8f,#9200ff);
    margin: -70px 30px 20px;
    color: #fff;
    text-align: center;
    font-size: 12px;
    border-radius: 10px;  
}
.middle-box h1
{
    padding-top: 30px;
    padding-bottom: 30px;
    font-size: 50px;
    font-weight: normal;
}
.middle-box h1 span
{
    font-size: 20px;
    margin-left: 5px;
    bottom: 18px;
    position: relative;
}
.payment-option-btn
{
    color: #fff;
    margin: 5px 30px;
    height: 30px;
    width: 290px;
    background-color: #9100fd;
    border: none;
    cursor: pointer;
}
.card-details
{
    background: #fff;
    color: #555;
    margin: 10px 30px;
    padding: 10px;
}
.card-detail p
{
    font-size: 14px;
}
.card-details label
{
    font-size: 10px;
    line-height: 20px;
}
.card-details label
{
    font-size: 10px;
    line-height: 20px;
}
.card-num-field-group
{
    margin-top: 10px;
}
.date-field-group
{
    margin-top: 10px;
    display: inline-block;
}
.cvv-field-group
{
    margin-top: 10px;
    display: inline-block;
    float: right;
}
.name-field-group
{
    margin-top: 10px;
}
.card-num-field, .name-field-group
{
    width: 270px;
}
.date-field, .cvv-field
{
    width: 80px;
}
.card-details input
{
    border: 1px solid #ccc;
    height: 22px;
    padding: 5px;
    font-size: 10px;
}
.card-details input::placeholder
{
    color:#ccc;
}
import "http://code.ionicframework.com/ionicons/2.0.1/css.min.css";
body
{
    margin: 0;
    padding: 0;
    font-family: sans-serif;
}
.btn
{
    position: absolute;
    width: 270px;
    margin-top: 20px;
    height: 30px;
    background-color: #9100fd;
    font-size: 20px;
    color: #fff;
    border: none;
    cursor: pointer;

}
#box
{
    width: 600px;
    overflow: hidden;
    background: #f1f1f1;
    box-shadow: 0 0 20px black;
    border-radius: 8px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
    z-index: 9999;
    padding: 10px;
    text-align: center;
    display: none;
}
#box span
{
    color: #2ecc71;
    font-size: 40px;
    display: block;
    margin: 20px 0;
}
#box h1
{
    color: #333;

}
.close
{
    font-size: 20px;
    color: white;
    padding: 10px 30px;
    cursor: pointer;
    background: #3498db;
    display: inline-block;
    border-radius: 4px;

}
</script>

