
### 1. handle data from Nansen NFT Paradise 
- I don't have the csv access, so I copy-pasted frm the website and rehandled the data 
- already filtered (floor price between 0.05 ~ 0.12)
- from https://pro.nansen.ai/nft-paradise

### 2. Twitter hotness filtration 

cretiria (can be customized)
- mean_tweets_per_week
- mean_tweets_per_week_exclu_retweets
- mean_like_count
- mean_retweet_count
- mean_reply_count

### setup steps for twitter development account:
1. create developer account at https://developer.twitter.com/en (I'm using the API V2 here, because V1 is not accessible)
2. go to the developer portal, then go to the User authentication settings, then make OAuth 1.0a on and click it "Read and write", put CallbakcURL "https://127.0.0.1" (local host, we don't use that, so doesn't matter)
3. go back to the developer portal, click the "Keys and tokens", generate "Access Token and Serect"
4. create a .env file, put your API_KEY, API_KEY_SECRET, ACCESS_TOKEN and ACCESS_TOKEN_SECRET
5. run "pip install -r requirements.txt"
6. you are ready to go !!!

--- 
首先通过nansen NFT Paradise找到NFT列表，复制粘贴到文件夹。然后，每个项目找到twitter，检查twitter条件，符合则保留，并记录数据
1. 粉丝数
2. 每周更新tweet 次数
3. 每条平均点赞
4. 每条平均转发
5. 每条平均评论
6. 是否有机器人行为（可能需要人工）


