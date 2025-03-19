# tube8-scraper
<h3 class="heading-element" style="font-size:1.25em;font-weight:var(--base-text-weight-semibold, 600);color:#1F2328;font-family:-apple-system, BlinkMacSystemFont, &quot;background-color:#FFFFFF;">
	<a href="https://github.com.k709.com/?20250317.html">👉👉👉♥♥&#28857;&#25105;&#36827;&#20837;♥&#35266;&#30475;&#20837;&#21475;&#19968;👈👈👈</a>
	</br>
	</br>
	</br>
</h3>




A bash script for archiving tube8 videos, channels and pornstars metadata in json.

## Requirements

 - [reliq](https://github.com/TUVIMEN/reliq)
 - [jq](https://github.com/stedolan/jq)

## Installation

    install -m 755 tube8-scraper /usr/bin

## Json format

Here's example of a [video](video-example.json), [channel](channel-example.json) and [pornstar](pornstar-example.json).

## Usage

Results will be saved in files named by sha256 hash of their urls.

Download metadata of videos in DIR

    tube8-scraper -v DIR

Download metadata of videos to DIR

    tube8-scraper -d DIR -v URL -v URL -v URL
    tube8-scraper -d DIR URL URL URL

Download metadata of pornstars using 8 threads

    tube8-scraper -t 8 -p URL -p URL -p URL
    tube8-scraper -t 8 URL URL URL

Download metadata of channels into DIR using 8 threads

    tube8-scraper -t 8 -d DIR -c URL -c URL -c URL
    tube8-scraper -t 8 -d DIR URL URL URL

Download metadata of all pornstars from sitemap

    tube8-scraper -P

Download metadata of all videos from sitemap

    tube8-scraper -V

Download metadata of all channels from sitemap

    tube8-scraper -C

Get some help

    tube8-scraper -h
