## Generating QR-Codes

Such as
![alt text](http://chart.apis.google.com/chart?cht=qr&chs=320x320&chl=http%3A%2F%2Fdjembe.ekomobi.com "Title")

for i in 0 1 2 3 4 5 6 7 8 9; do curl "http://chart.apis.google.com/chart?cht=qr&chs=320x320&chl=http%3A%2F%2Fdjembe.ekomobi.com/$i" >QR-djembe-$i.png; done

or

while true; do r=$RANDOM; curl "http://chart.apis.google.com/chart?cht=qr&chs=320x320&chl=http%3A%2F%2Fdjembe.ekomobi.com/$r" >QR-djembe-$r.png; done

while true; do r=$RANDOM;s=$RANDOM;t=$RANDOM; curl "http://chart.apis.google.com/chart?cht=qr&chs=320x320&chl=http%3A%2F%2Fdjembe.ekomobi.com/$r$s$t$r$s$t$r$s$t$r$s$t$r$s$t" >QR-djembe-$r$s$t.png; done


while true; do r=$RANDOM;s=$RANDOM;t=$RANDOM;u="$r$s$t"; curl "http://chart.apis.google.com/chart?cht=qr&chs=320x320&chl=$u$u$u$u$u$u$u$u" >QR-djembe-$u.png; done

javascript:setInterval(function(){r=Math.random;window.location="http://chart.apis.google.com/chart?cht=qr&chs=320x320&chl="+r()},1000)