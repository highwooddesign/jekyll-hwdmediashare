---
layout: post
title:  "PHP 7 Support"
date:   2016-04-14 20:08:44 +0100
categories: Docs jekyll update
---
<div class="item-page" itemscope="" itemtype="https://schema.org/Article"><meta itemprop="inLanguage" content="en-GB">

<div class="page-header">

## PHP7 Support

</div>

<dl class="article-info muted">

<dt class="article-info-term">Details</dt>

<dd class="article-meta" itemprop="author" itemscope="" itemtype="http://schema.org/Person">Written by <span itemprop="name">Dave Horsfall</span>, <time datetime="2016-04-14T15:59:55+01:00" itemprop="datePublished">Thursday, 14 April 2016</time></dd>

</dl>

<div class="disqus-count">[1 Comment](/blog/767-php7-support#disqus_thread)</div>

<div class="pull-none item-image">![](/images/site/blog/767/php7.png)</div>

<div itemprop="articleBody">

Joomla 3.5 was released [last week](https://www.joomla.org/announcements/release-news/5654-joomla-3-5-is-here.html). This new version included lots of lovely features, but one which many of our community have asked about is support for PHP7\. Joomla now includes support for the recently released PHP7 scripting language, and the aim of this post if to clarify the support for HWDMediaShare. PHP7 was recently announced with [significant performance improvements](https://www.gavick.com/blog/joomla-php-7-speedtest) and is now available for use by the general public. Joomla can run twice as fast and with half the memory usage on systems that run PHP7, so we understand why people are excited about this major new release of PHP.

We can now confirm that HWDMediaShare 2.0.5 is compatible with Joomla 3.5 and PHP7.

## Joomla Performance Tests

There are many articles offering detailed Joomla performance tests for the new PHP7, but we'll do a quick comparison for HWDMediaShare pages. These tests are run on a localhost server using WAMP. The PHP versions which have been compared are **PHP 5.6.16**, and **PHP 7.0.0**. The Joomla page being tested is the HWDMediaShare media view. 

### PHP6

The total load time (afterRender event) was 936.05ms and consumed 15.87MB of memory.

![](/images/site/blog/767/profile-php6.png)

### PHP7

The total load time (afterRender event) was 505.03ms and consumed 11.65MB of memory.

![](/images/site/blog/767/profile-php7.png)

## Performance Test Comparisons

<table class="category table table-striped table-bordered table-hover">

<tbody>

<tr>

<td> </td>

<td>**PHP 5.6.16**</td>

<td>**PHP 7.0.0**</td>

</tr>

<tr>

<td>****Load Time****</td>

<td>936.05ms</td>

<td>505.03ms</td>

</tr>

<tr>

<td>**Memory Usage**</td>

<td>15.87MB</td>

<td>11.65MB</td>

</tr>

</tbody>

</table>

These tests demonstrate that making the switch to PHP7 **<span class="output-n4">reduces the load time by 46% and saves</span> **<span class="output-n4">**27% of memory**.</span>

</div>

<div id="disqus_thread"><iframe id="dsq-app7900" name="dsq-app7900" allowtransparency="true" frameborder="0" scrolling="no" tabindex="0" title="Disqus" width="100%" src="https://disqus.com/embed/comments/?base=default&amp;f=hwdmediashare&amp;t_i=c975d60935_com_content_article_767&amp;t_u=https%3A%2F%2Fhwdmediashare.co.uk%2Fblog%2F767-php7-support&amp;t_d=PHP7%20Support&amp;t_t=PHP7%20Support&amp;s_o=default&amp;l=en#version=b540e7baf9f0093a713fc183a7078c20" horizontalscrolling="no" verticalscrolling="no" style="height: 375px !important;"></iframe></div>

<script type="text/javascript">var disqus_shortname = 'hwdmediashare'; var disqus_url = 'https://hwdmediashare.co.uk/blog/767-php7-support'; var disqus_identifier = 'c975d60935_com_content_article_767'; var disqus_config = function(){ this.language = 'en'; }; (function() { var dsq = document.createElement('script'); dsq.type = 'text/javascript'; dsq.async = true; dsq.src = '//' + disqus_shortname + '.disqus.com/embed.js'; (document.getElementsByTagName('head')[0] || document.getElementsByTagName('body')[0]).appendChild(dsq); })();</script>

<noscript>Please enable JavaScript to view the [comments](//disqus.com/?ref_noscript)</noscript>

</div>