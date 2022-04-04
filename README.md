Hi Guys , Welcome 


![noun-astronaut-3769126-71D358](https://user-images.githubusercontent.com/102995746/161629096-4a13bb2f-d5dc-43d9-9f72-b9d54e35f6ea.png)




*:Web Security 
>chalange name : R2D2 -Easy -web security

![1_bEAExeSgZ1JRdn9RTg6jiA](https://user-images.githubusercontent.com/102995746/161623787-3abb3172-7ee1-4ad2-95c3-e6f8f84924ed.png)

After enter the chalange we got photo of 2 robots i think this is Hint , also before i solve any web ctf i tried first testing for common files/folders like /robots.txt , /.git ,/admin
so  i tested robots.txt and here we go 
and the flag in /robots.txt
.........................................
Flag :shctf{th1s-aster0id-1$-n0t-3ntir3ly-stable}  
........................................
 >>>chalange name : Space Buds - medium - web security 


![Screenshot_1](https://user-images.githubusercontent.com/102995746/161624455-36b3a4e4-d3c3-4b65-8f98-2cb3bcda2f7c.png)

before we enter he chalange we have this photo and told us that "one of the puupies got into the web server " ammm ok
if we access the website, i think  is nothing interesting but we have name"userID" and value of cookie "whoami" i think the play in value of cookie and we know "one of puppies got into srever" so i tried to search name of dogs in this film and i try with "Mudbud" name of one dogs in film and here we go 


![mudbud](https://user-images.githubusercontent.com/102995746/161625649-44f13232-c5fd-40c7-a5fa-ed8eada0499d.png)


...............................
Flag :shctf{tastes_like_raspberries}
...............................

>chalange name : Space Traveler - Easy - web security 

i start to look in Source Code and only interesting thing in source is JavaScript var 


![Screenshot_3](https://user-images.githubusercontent.com/102995746/161626313-2a915983-2402-44bf-9355-db18fe0d2ef1.png)


we can use beautifier.io to beautify the code and here we go 


![Screenshot_4](https://user-images.githubusercontent.com/102995746/161626870-63229e75-f935-4107-9350-d85026eb7909.png)


..........................................
Flag :shctf{eighty_seven_thousand_million_suns}
.......................................


>chalange name : Mysterious Broadcast - Hard - web security

when acess the chalange we have this sign ~ and nothing in source code no files or directory but when i refresh page i got nmber 1 ammm i refresh again and again and i see the page give me number 0 or 1 




![reload](https://user-images.githubusercontent.com/102995746/161627389-d3a60395-350f-49c9-8837-4fb4b62a261b.png)





i start to collect this number 
by

for ((i=1;i<300;i++)); do curl http://173.230.134.127/seq/ad9ce99a-4e54-4a4d-a0fc-a26b2866f5d8; done 

and i see ~ is repeated after some numbers and go in loop so i choose numbers from ~ to ~ and i got this
1100011011001011010001101010110010010001111011010011011110100011011000100111011010101100001101011111011001001010110001101100001000101011001110100011101101110110001100001010101011001110100101101000110001011011011010010110100011000111101101101001001110011000011110011101111010111101

i used decode.fr to identify type of encoding and this is BIN7bit ASCII i decoded this and i got Base64"c2hjdGZ7QXNjaWlJc0E3Qml0U3RhbmRhcmR9Cg==
" i decoded and here we go 

![Screenshot_5](https://user-images.githubusercontent.com/102995746/161627891-0d011dcc-ed2e-4b9c-992e-1ac254d3b704.png)



![Screenshot_6](https://user-images.githubusercontent.com/102995746/161627897-aedabf49-6fb9-4c4c-9135-3c4ce80ee205.png)


...................
Flag : shctf{AsciiIsA7BitStandard}
...................


>chalange name : Flag in Space - Easy - web security
after access chalenge we got this url http://172.105.154.14/?flag=
i try to add shctf in flag parameter and print it on the page so i think what should we will do i we will guess evers numbers or characters in the flag by using burb intruder 


![grid](https://user-images.githubusercontent.com/102995746/161628349-ba9fac90-0c79-4aaf-b3b5-359a6f46de74.png)



![Screenshot_7](https://user-images.githubusercontent.com/102995746/161628573-09ed44fc-f048-4677-a8d2-f67a17eee1c0.png)



![1_l0ec9QgsSDHdbG4mTRcfeA](https://user-images.githubusercontent.com/102995746/161628768-2c1d95ab-3f90-479a-9225-b681e87b1a48.png)


diiferent lenght meean charcters found


an here we go 

shctf{2_explor3_frontier}



bye





