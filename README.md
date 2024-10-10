# hello-starknet-foundry

snforge init project_name
snforge test


sncast
--profile myprofile

sncast --profile myprofile \
    call \
    --contract-address <contract address> \
    --function get \
    --calldata 0x0 \
    --block-id latest



## 笔记
创建帐号
```
sncast \
account create  \
--url http://127.0.0.1:5050 \
--class-hash 0x061dac032f228abef9c6626f995015233097ae253a7f72d68552db02f2971b8f \
--type oz \
--name dev \
--add-profile dev
```

部署账号
```
sncast \
account deploy  \
--url http://127.0.0.1:5050 \
--name dev \
-v v1 \
--fee-token eth
```