# Ranked Love
<a href="https://brennan.games/RankedLove/">Coming soon to ``brennan.games/RankedLove``</a><br />

This app is a celebration of the complex emotions we experience in relationships, particularly jealousy—a deeply misunderstood and often vilified feeling. Rather than fearing or suppressing it, this project radically embraces jealousy as a beautiful and powerful emotion. Jealousy can remind us of our capacity for love, desire, and care—a reflection of how much someone matters to us. The app challenges cultural norms that glorify control, possessiveness, and toxic behaviors around jealousy. Instead, it asks us to explore healthier, more creative ways to experience and express these feelings, normalizing openness and love for multiple people without restriction.

## Setup 
### Server Setup

AWS Lightsail NodeJS<br />
#### Setup Security
IPv4 Firewall: Custom	TCP	3000 Any IPv4 address<br />
IPv6 firewall: Custom	TCP	3000 Any IPv6 address<br />

### Installing Requirements 

Replace the ``/opt/bitnami/apache/conf/bitnami/bitnami-ssl.conf``<br />
``sudo /opt/bitnami/ctlscript.sh restart apache``<br />
<br />
````npm install -g pm2````<br />
``npm installc cors``<br />
``npm install express``<br />
``npm install axios``<br />
``npm install elevenlabs-node``<br />
``npm install play-sound``<br />
``npm install sqlite3``<br />
``npm install dotenv``//cant tell if I am using this<br /> 
``npm install multer``
``npm install form-data``
Put evnionment variables into ``env.js``
Looking like this
```const ENV = {};
ENV.TNL_API_KEY = 'XXXX';
ENV.OPENAI_API_KEY = 'XXXX';
ENV.ELEVENLABS_API_KEY = 'XXXX';

module.exports = ENV;
```

Public Client Setup
``npm i bootstrap@5.3.0``<br />

## Run
Move into the server folder.
Run ``pm2 start ecosystem.config.js``
Check status ``pm2 status``
Check log ``pm2 log``

## Update

### Wed 18 Dec 2024
Did a <a href="https://www.facebook.com/brennan.hatton/posts/pfbid0oLbRezQTLm5CWLhUknMHXqfDQ9t4QNAkPCirxuGvtoEt9wy3TqXnyiFBxQzjNDERl">facebook post</a> and survey asses it as a product. I learnt that a lot of people hate this idea, but there is some part of how bold the controversy is that I like. I feel like it highlights projections of insecurities which in itself is some kind of art piece.
