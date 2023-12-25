## **PRC-520 deploy，mint，transfer**

\*\*1.deploy\
\*\*{

"p": "prc-520",

"op": "deploy",

"tick": "",

"max": "",

"lim": "",

"to": "",

"fee": "",

}

·  p The first character of “protocol”, telling the resolver it’s a PRC-520 protocol.

·  op Type of event

·  tick Name

·  max Set maximum supply

·  lim Mint limitation

·  to Receiver

·  fee Handling fee

 

 

\*\*2.mint\
\*\*{

"p": "prc-520",

"op": "mint",

"tick": "",

"amt": ""

}

·  p The first character of “protocol”, telling the resolver it’s a PRC-520 protocol.

·  op Type of event

·  tick Name

·  amt Minted amount

 

 

\*\*3.transfer\
\*\*{

"p": "prc-520",

"op": "transfer",

"tick": "",

"amt": ""

}

·  p  The first character of “protocol”, telling the resolver it’s a PRC-520 protocol.

 

·  op Type of event

·  tick Name

·  amt Designated PRC-520 amount to be transferred

 





## **prc-520 index rules**

(1)deploy

{

"p": "prc-520",

"op": "deploy",

"tick": "",

"max": "",

"lim": "",

"to": "",

"fee": "",

}

·  p The first character of “protocol”, telling the resolver it’s a PRC-520 protocol.

·  op Event typre

·  tick Name

·  max Set maximum supply of prc-520

·  lim Minting limitation

·  to Receiver

·  fee Handling fee

 

inscription\_utf8(Inscription content transcript JSON)

  data:,{ "p": "prc-520","op": "deploy","tick": "","max": "","lim": "","to": "","fee": "",}

Note: to and fee should be included to finish the check

 

(2)mint\
{

"p": "prc-520",

"op": "mint",

"tick": "",

"amt": ""

}

·  p The first character of “protocol”, telling the resolver it’s a PRC-520 protocol.

 

·  op  Event type（deploy, mint, transfer）

·  tick Name

·  amt Minting amount

 

inscription\_utf8(Inscription content transcriptJSON)

data:,{"p":"prc-520","op":"mint","tick":"","amt":""}

inscription(content of inscription)

e.g.: 0x646174613a2000000000000000000000000022c22616d74223a2231303030227d

 

To Receiver

 

Fee Handling fee

 

type

The last digit of the hash value generated when minting as type, 36 types in total(0-9, A-Z)

 

hash

e.g.：0x760ac8b989b60000000000000088600000000300000b3f

 

Note: Mint needs to satisfy correct To, Fee and inscription content to be correctly indexed

 

 

 

(3)transfer

 

{

"p": "prc-520",

"op": "transfer",

"tick": "",

"amt": ""

}

·  p The first character of “protocol”, telling the resolver it’s a PRC-520 protocol.

·  op Event type（deploy, mint, transfer）

·  tick Name

·  amt Designated PRC-520 amount to be transferred

 

inscription\_utf8(Inscription content transcript JSON)

data:,{"p":"prc-520","op":"transfer","tick":"","amt":""}

 

 

Note: transfer needs to satisfy correct inscription content to be correctly indexed

 
