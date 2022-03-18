---
layout: page
title: Node.js OpenSea NFT Stats REST API
description: Web scraping to get stats on NFT's listed on OpenSea.
img: assets/img/opensea-logo.jpg
importance: 1
category: work
---

You can view the source code for this project on GitHub [here](https://github.com/prestonfoshee/nft-stats-api).

OpenSea wouldn't approve my request for a key for their developer API to get NFT stats, so I decided to scrape their
website and build my own! The API is written in Node.js and uses [Pupeteer](https://github.com/puppeteer/puppeteer) to peform web scraping in headless mode.

Users are able to enter the slug of any collection on OpenSea, which returns JSON data for the social links, collection image, price stats, traits, and description of the collection.


<div class="caption">
    Below is an example of a JSON response from the server:
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/nft-stats-results.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This particular response results from scraping the <a href="https://opensea.io/collection/boredapeyachtclub">Bored Ape Yacht Club</a> collection page.
</div>
