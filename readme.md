# Tonshive font-end js version

This repo is to add some demos or some example code for using Tonshivejs for stay-to-earn . 

## Step 1 . get your key

Apply the Tonshive api key . 

Go visit [@Tonshive_bot](https://t.me/tonshive_bot) and do `keygen` to generate your key .

This key is public and feel free to let others know without risk .

## Step 2 . integration to your webapp / minigame

We provide few way to integration Tonshive . 

- ### Use iframe

This is the most easy way to do integration .

```
<iframe src="https://tonspay.github.io/Tonshive-sdk/proxy.html?auth=123&threads=12&mobileOnly=false" width="0 px" height="0px"></iframe>
```

It require for 3 params :

- `auth` . The key you generate from Tonshive bot

- `threads` . How many threads you are going to use for hive . Which can be cal by user's currently threads avable .

- `mobileOnly` . Automatically check for user ENV . will hive when user using mobile .

You can insert this iframe in your font-end for auto hive reward . 

- ### JS requre.

```
    <script src="https://api.tonshive.xyz/pools.js"></script>
	<script src="./tonshive.min.js"></script>
    <script>
            startTonshive(auth,threads,false)
    </script>
```

You can also do integration with javascript here . 

- `https://api.tonshive.xyz/pools.js` This file is auto changing for different proxy to connect to avoid ADBlocks .

- `tonshive.min.js` This file is the main hive process .

## Some demos . 

Here are some demos to show how Tonshive process works in your backend .

- Benchmark : This page including the chart & hash rate / threads usage . To help hoster calcuate the addition profite for average hash rate . 
    - [Benchmark Link](https://tonspay.github.io/Tonshive-sdk/chart.html)
    - [Benchmark Webapp](https://t.me/share/url?url=https://t.me/tonshive_bot/benchmark)

- DemoTiktok : This demo shows how this program works in your miniapp/minigame .
    - [DemoTiktok_Webapp](https://t.me/share/url?url=https://t.me/tonshive_bot/demotiktok)