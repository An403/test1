<?php
$d = 10;
?>

<html>
<head>
    <meta charset="utf-8">
    <style>
        .f-c{
            background: red;
        }
        .f-v{
            background: pink;
        }
        th, td{
            padding: 10px;
        }
    </style>
</head>
<body>
    <table>
        <thead>
            <th class="f-c"></th>
            <?for($i = 1; $i <= $d;$i++):?>
                <th class="f-c"><?=$i?></th>
            <?endfor;?>
        </thead>
        <tbody>
            <?for($i = 1; $i <= $d;$i++):?>
                <tr>
                    <th class="f-c"><?=$i?></th>
                    <?for($j = 1; $j <= $d;$j++):?>
                        <th class="f-v"><?=$i*$j?></th>
                    <?endfor;?>
                </tr>
            <?endfor;?>
        </tbody>
    </table>
</body>
</html>
