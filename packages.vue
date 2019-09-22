<template>
    <div class="South Indian Heitage Express">
    <p>
        <link rel="stylesheet" href="css/font-awesome.min.css"/>
    </p>

    <script>
        $(document).ready(function() {
        $("#more-details").on("click",function(){
            $.getJSON("/trains_name.json",function(json){

            var htm ="";
            json.foreach(function(val){
                var keys = object.keys(val);
                    htm += "<div class ='more-details'>";
                    htm += "<package_id='" + val.packages_id + "'" + "train_name='" + val.train_name +" ' " + "train_id='" +val.train_id + "'" + "stops_id'" + val.stops_id +"' width='23%' heigth='40%'><br>"
                    keys.foreach(function(key){
                        htm +="<strong>" + key + "</strong>: " + val[key]+ "<br>";
                    });
                    htm +="</div><br>";
                });
                $(".data").html(htm);      
            });
        });
        });
    </script>
        <div class="container">
            <div class="app">
                <div class="nav">
                    <i class="fa fa-bars"></i><i class="fa fa-Packages"></i><i class="fa fa-search"></i>
                </div>
                <div class ="list-items">
                    <div class="list-items">
                        <img src="img.jpg" alt=""width="110">
                    </div>
                    <a href="login.html">
                    <span class="book-now">
                        <i class ="fa fa-ticket"></i>
                    </span>
                    </a>
                    <div class ="train-details">
                        <div class =" short-detail">
                            <table>
                                <tr>
                                    <td class="title">Coastal_Breeze</td>
                                </tr>
                                <tr>
                                    <td class="from">Chennai</td>
                                    </td>
                                </tr>
                            </table>
                            <span class="more-datails"></span>
                        </div>
                    </div>
                </div>
                <div class ="list-item  s">
                    <div class="list-items">
                        <img src="img.jpg" alt=""width="110">
                    </div>
                    <a href="login.html">
                    <span class="book-now">
                        <i class ="fa fa-ticket"></i>
                    </span>
                    </a>
                    <div class ="train-details">
                        <div class =" short-detail">
                            <table>
                                <tr>
                                        <td class="title">Vijayanagar Experience</td>
                                 </tr>
                                 <tr>
                                     <td class="from"> From Bengaluru</td>
                                     </td>
                                 </tr>
                            </table>
                            <span class="more-details"></span>
                        </div>
                     </div>
                 </div>
                <div class ="list-items">
                        <div class="list-items">
                            <img src="img.jpg" alt=""width="110">
                        </div>
                        <a href="login.html">
                        <span class="book-now">
                            <i class ="fa fa-ticket"></i>
                        </span>
                        </a>
                        <div class ="train-details">
                           <div class =" short-detail">
                                <table>
                                     <tr>
                                          <td class="title">Deccan Dilbaug</td>
                                     </tr>
                                     <tr>
                                           <td class="from">From Mumbai</td>
                                     </tr>
                                 </table>
                               <span class="more-datails"></span>
                            </div>
                         </div>
                 </div>
                <div class ="list-items">
                    <div class="list-items">
                          <img src="img.jpg" alt=""width="110">
                    </div>
                    <a href="login.html">
                    <span class="book-now">
                        <i class ="fa fa-ticket"></i>
                    </span>
                    </a>
                    <div class ="train-details">
                        <div class =" short-detail">
                             <table>
                                 <tr>
                                      <td class="title">Eastern Seascape</td>
                                 </tr>
                                 <tr>
                                     <td class="from">From Hyderabad</td>
                                      </td>
                                 </tr>
                             </table>
                             <span class="more-details"></span>
                        </div>
                     </div>
                  </div>
            </div>
        </div>
    </div>
</template>

<style scoped>

*
{
    margin: 0;
    padding: 0;
    outline: none;
}

body
{
    font-family: sans-serif;
    overflow: hidden;
    background: #1e2535;
}
.container
{
    width: 430px;
    height: 900px;
    margin: 0px auto;
    margin-left: 975px;
    display: inline-block;
}
div.app
{
    position: relative;
    width: 365px;
    height: 700px;
    backface-visibility: #6a18ff;
    margin-top: 30px;
    overflow: hidden;
    box-shadow: inset -15px -15px 80px rgba(0,0,0,.15);
    perspective: 500px;
}
div.app:before
{
    position: absolute;
    content: '';
    width: 300%;
    height: 100%;
    background: rgba(255,255,255,0.92);
    bottom: -30px;
    transform-origin: left bottom;
    transform: rotate(-10deg);
    z-index: -1;
}
div.nav
{
    position: absolute;
    width: 100%;
}
div.nav div.nav-top
{
    padding-top: 15px;
    padding-bottom: 28px;
    width: 100%;
}
div.nav div.nav-top i
{
    width: 33.33%;
    color: #fff;
    font-size: 21px;
    opacity: 0.5;
}
div.nav div.nav-top i:last-child
{
    width: 30%;
    text-align:right;
}
div.nav div.nav-top i:nth-child(2)
{
    position: relative;
    opacity: 0.95;
    text-align: center;
    top: -1px;
}
div.nav div.nav-top i:first-child
{
    width: 30%;
    margin-left: 15px;
}
div.nav::before
{
    position: absolute;
    content:'';
    width: 100%;
    height: 85%;
    box-shadow: inset 0 65px 55px -25px rgba(0,0,0,0.3);
}
div.list-item
{
    position: relative;
    top: 100px;
}
div.list-item
{
    position: relative;
    margin-bottom: 25px;
    padding: 0 0 0 3%;
}
div.list-thumb
{
    position: absolute;
    width: 110px;
    height: 110px;
    overflow: hidden;
    border-radius: 10px;
    transform: scale(0.85)translate(0px);
    box-shadow: 10px 15px 15px -10px rgba(0,0,0,.2);
    opacity: 1;
    z-index: 1;
}
div.list-item span.train-time-left
{
    position: absolute;
    font-size: 11px;
    font-weight: 600;
    bottom: -5px;
    left: 20px;
}
div.list-item span.book-now
{
    position: absolute;
    top: 0;
    right: 0;
    z-index: 1;
    font-size: 40px;
    font-weight: 600;
    color: rgba(255,255,255,0.95);
    background: #6a18ff;
    width: 60px;
    height: 48px;
    background-image: url('');
    line-height: 48px;
    text-align: center;
    border-radius: 10px;
    margin-top: 80px;
    transform: translate(-15px);
    box-shadow: 0 18px 15px -10px rgba(106,24,255,.5),
                0 18px 15px -10px rgba(0,0,0,0.05);
    border-bottom: 1px solid rgba(0,0,0,0.1);
    border-top: 1px solid rgba(0,0,0,0.1);
    display: none;
}
div.list-item span.book-now i
{
    transform: rotate(45deg);
}
div.train-details
{
    width: 97%;
    top:0;
    z-index: -1;
    height: 120px;
    transform: translateY(25px);
}
div.train-details div.short-detail
{
    position: absolute;
    left: 0;
    width: 45%;
    background: #fff;
    display: inline-block;
    padding: 15px 45px;
    padding-right: 55px;
    border-radius:5px;
    transform-origin: left bottom;
    transform: translateX(75px) scaleY(1);
    box-shadow: 0 25px 45px -10px rgba(0,0,0,.3);
    opacity: 1;
}
div.train-details div.short-detail td
{
    padding: 1px 0;
}
div.train-details div.short-detail .title
{
    font-size: 19px;
    font-weight: 700;
    letter-spacing: 0.2px;
    color: rgba(0,0,0,.8);
}
div.train-details div.short-detail .from
{
    font-size: 15px;
    font-weight: 500;
    letter-spacing: 0.2px;
    color: rgba(0,0,0,.4);
}
div.train-details div.short-detail span.more-option
{
    position: absolute;
    width: 4px;
    height: 4px;
    display: inline-block;
    background: rgba(0,0,0,.2);
    right: 20px;
    top: 20px;
    border-radius: 100%;
    box-shadow: 0 6px 0 rgba(0,0,0,.2)
                0 12px 0 rgba(0,0,0,.2);
}
div.list-item:nth-child(2),
div.list-item:nth-child(3),
div.list-item:nth-child(4)
{
    display: none;
}
</style>