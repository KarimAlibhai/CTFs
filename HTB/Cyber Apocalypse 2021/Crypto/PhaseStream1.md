## PhaseStream1

Method: We know that the key is 5 bytes, we also know the text contains CHTB{
Thus we can deduce the first 5 bytes xored with CHTB{ will give us the key (as CHTB{ is also 5 bytes)

![image](https://user-images.githubusercontent.com/61699641/116566909-0f321780-a8ff-11eb-95bc-6345661a385b.png)

Looking at the output for the first 5 bytes the key is shown as 'mykey'

Plugging it back in:

![image](https://user-images.githubusercontent.com/61699641/116566970-1e18ca00-a8ff-11eb-8894-b7d308a20a3b.png)

Flag: CHTB{u51ng_kn0wn_pl41nt3xt}

Challenge solved by Karim
