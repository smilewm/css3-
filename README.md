##html
 < ul class="demo" ><br/>
 &nbsp;&nbsp;&nbsp;&nbsp;< li >< /li ><br/>
 < /ul >
##css3
<pre>
    * {
      padding: 0;
      margin: 0;
    }

    .demo {
      list-style: none;
      width: 100%;
      height: 180px;
      text-align: center;
    }

    .demo li {
      position: relative;
      width: 20%;
      height: 100%;
      margin-right: 3%;
      background: #f60;
      display: inline-block;
    }

    .demo li:before,
    .demo li:after {
      content: "";
      position: absolute;
      top: -20px;
      display: block;
      width: 10px;
      height: 100%;
      margin-top: 20px;
      background-size: 20px 10px;
    }

    .demo li:before {
      left: -10px;
      background-color: #fff;
      background-position: 100% 35%;
      background-image: linear-gradient(-45deg, #f60 25%, transparent 25%, transparent),
        linear-gradient(-135deg, #f60 25%, transparent 25%, transparent),
        linear-gradient(-45deg, transparent 75%, #f60 75%),
        linear-gradient(-135deg, transparent 75%, #f60 75%);
    }

    .demo li:after {
      right: -10px;
      background-color: #f60;
      background-position: 100% 15%;
      background-image: linear-gradient(-45deg, #fff 25%, transparent 25%, transparent),
        linear-gradient(-135deg, #fff 25%, transparent 25%, transparent),
        linear-gradient(-45deg, transparent 75%, #fff 75%),
        linear-gradient(-135deg, transparent 75%, #fff 75%);
    }
</pre>