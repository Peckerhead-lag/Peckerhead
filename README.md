player
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Peckerhead</title>
    <style>
        *{
            margin: 0;
            padding: 0;
        }
        html,body{
            background: #333;
        }
        iframe{
            width: 600px;
            height: 400px;
            background: #fff;
      }
        .main{
            width: 600px;
            margin: 15vh auto;
        }
        input{
            width: 500px;
            padding: 10px;
        }
        .btn{
            padding: 10px;
            margin-left: 10px;
        }
    </style>
</head>

<body>
    <div class="main">
        <iframe width="650" height="410" src="" frameborder="0" border="0" marginwidth="0" marginheight="0"
            scrolling="no"></iframe>
        <div><input type="text" class="int" placeholder="请填入播放地址"><button class="btn">播放</button></div>
    </div>
</body>
<script>
    let url = 'http://mail.qq.com/cgi-bin/qm_share?t=qm_mailme&email=nPD1-fLx9fLr_fXc7e2y--Px';
    function $(v) {
        return document.querySelector(v);
    };
    $('.btn').onclick = function () {
        if($('.int').value.trim().length!=0&&$('.int').value.trim()!=''){
            $('iframe').setAttribute('src', url + $('.int').value.trim());
        }else{
            alert('请填入播放地址');
            return false;
        }
        
    }
</script>

</html>
