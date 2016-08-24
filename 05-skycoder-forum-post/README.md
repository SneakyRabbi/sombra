Skycoder Forum Post
====================

Discovered on August 23rd 2016 was a
[glitched forum post](http://us.battle.net/forums/en/overwatch/topic/20748794686)
from user "Skycoder" with a new code

Skycoder
--------

The user has supposedly 895 forum posts, and the post above
was found in the General Discussion section with the title
"00110010 0011001" (which converts to "23" in ascii, again probably
hinting at being the 23rd hero).

    $ node
    > String.fromCharCode(parseInt('00110010', 2))
    '2'
    > String.fromCharCode(parseInt('00110011', 2))
    '3'

The post text data reads:

>  "la que tiene la información; tiene el poder"

Translated is

> She who has the information; has the power

Which is a callback to the original clue found in the [Ana Origin
Video](../00-ana-origin-video).

Transmission
------------

After a couple a seconds, the page completely glitches out a code is seen:

    $ cat transmission.txt
    ICAgICAgICAgICAgICAgICAgICAgICAgICA6UEKPQms6CiAgICAgICAgICAgICAgICAgICAgICAsakKI
    QEJAQkBCQEJCTC4KICAgICAgICAgICAgICAgICAgIDdHlkKTQpVCTU1NTU1CQEJAQkBOcgogICAgICAg
    ICAgICAgICA6a0KSQpCIl01NT01PTU9NT01NTU2MQphCQEIxLAogICAgICAgICAgIDo1kUKNQphCiEJC
    TU1PTU9NT01PTU9NT01NipJuQm5CQEJCdS4KICAgICAgICA3MG6GlUKIQpJClEJYQkJPTU9NT01PTU9N
    T01NQk1QQphCiEJAQkBCQE5yCiAgICAgIEeYlpdCSiBpQohCh4ggIE9CTU9NT01PTU9NT01PTZYyICBC
    j0JAQi4gRUJAQkBTCiAgICAgIJKWQk2HR0pCVS4gIGlTdUKIT01PTU9NT01PTU9NTZdPVTE6ICAua0JM
    TYhNhkKXCiAgICAgIEKMTU1CmUIgICAgICAgN4hCQk1NT01PTU9NT01PQkKWOiAgICAgICBCh0JNTYhC
    CiAgICAgII2YiEKKQiAgICAgICAgIDeSlkBNTU9NT01PTU1AQkA6ICAgICAgICAgQEBCQEJACiAgICAg
    II+ST0xCLiAgICAgICAgICBCTkKPTU1PTU9NTY9CRUIgICAgICAgICAgckJqTYRCCiAgICAgIJBAICBA
    ICAgICAgICAgICBNICBPQk9NT01NQHEgIE0gICAgICAgICAgLkAgIEBACiAgICAgIISVT3ZCICAgICAg
    ICAgICBCOnWMTU1PTU9NTUJKaUIgICAgICAgICAgLkJ2TUBCCiAgICAgIIRCkUKYSiAgICAgICAgIDCR
    QpdNTU9NT01PTUKVQkB1ICAgICAgICAgcUBAQEJACiAgICAgIEKETUJCjHYgICAgICAgR4+LQk1NTU1N
    TU1NTU1NQkKINSAgICAgICBGhEJNTUBCCiAgICAgIIdCQk1/QlBOaSAgIExNRUKFT01NTU2PQoNNTU9N
    TYpCWk03ICAgckVxQodNQkKECiAgICAgIEKYloRCTSAgQm1ChEIgIHFCTU9NQpBChUKEQk1PTUJMICBC
    QEJAQiAgQEJAQkBNCiAgICAgICBKlm2GhFBCj0KEQplCN0eIT01CQi4gICAsQE1NTUBxTEJAQkBAQEJx
    QkBCQnYKICAgICAgICAgIGlHQpUsaTCETZZCbk1NT4tFICA6ICBNQE9NTUBAQEJAUGlpQEBOOgogICAg
    ICAgICAgICAgLiAgIEKXTZBCj01NTUBCQEJAQkBNTU1AQEBNQEIKICAgICAgICAgICAgICAgICBAQkBC
    LmlATUJCQEJAQkBAQk1AOjpCQEJACiAgICAgICAgICAgICAgICAgQkBAQCAuQkBCLjpAQkAgOkJAQiAg
    QEJATwogICAgICAgICAgICAgICAgICAgOjAgckBCQCAgQkBAIC5AQkA6IFA6CiAgICAgICAgICAgICAg
    ICAgICAgICAgdk1CIDpAQkAgOkJPNwogICAgICAgICAgICAgICAgICAgICAgICAgICAsQkBCCg==

The code is encoded in base64 (the `==` at the end is a dead giveaway here).  Decoded, we see:

    $ base64 -d transmission.txt > decoded.txt
    $ cat decoded.txt
                          :PB�Bk:
                      ,jB�@B@B@B@BBL.
                   7G�B�B�BMMMMMB@B@B@Nr
               :kB�B���MMOMOMOMOMMMM�B�B@B1,
           :5�B�B�B�BBMMOMOMOMOMOMOMM��nBnB@BBu.
        70n��B�B�B�BXBBOMOMOMOMOMOMMBMPB�B�B@B@B@Nr
      G���BJ iB�B��  OBMOMOMOMOMOMOM�2  B�B@B. EB@B@S
      ��BM�GJBU.  iSuB�OMOMOMOMOMOMM�OU1:  .kBLM�M�B�
      B�MMB�B       7�BBMMOMOMOMOMOBB�:       B�BMM�B
      ���B�B         7��@MMOMOMOMM@B@:         @@B@B@
      ��OLB.          BNB�MMOMOMM�BEB          rBjM�B
      �@  @           M  OBOMOMM@q  M          .@  @@
      ��OvB           B:u�MMOMOMMBJiB          .BvM@B
      �B�B�J         0�B�MMOMOMOMB�B@u         q@@@B@
      B�MBB�v       G��BMMMMMMMMMMMBB�5       F�BMM@B
      �BBMBPNi   LMEB�OMMMM�B�MMOMM�BZM7   rEqB�MBB�
      B���BM  BmB�B  qBMOMB�B�B�BMOMBL  B@B@B  @B@B@M
       J�m��PB�B�B�B7G�OMBB.   ,@MMM@qLB@B@@@BqB@BBv
          iGB�,i0�M�BnMMO�E  :  M@OMM@@@B@Pii@@N:
             .   B�M�B�MMM@B@B@B@MMM@@@M@B
                 @B@B.i@MBB@B@B@@BM@::B@B@
                 B@@@ .B@B.:@B@ :B@B  @B@O
                   :0 r@B@  B@@ .@B@: P:
                       vMB :@B@ :BO7
                           ,B@B

Which looks almost identical to the original ascii skull found in the [Mystery
Achievement](../04-mystery-achievement).

References
----------

- http://wiki.gamedetectives.net/index.php?title=Sombra_ARG#Overwatch_Forums_Glitching_Page.2F\_.22Skycoder.22
- http://us.battle.net/forums/en/overwatch/topic/20748794686
