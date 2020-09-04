---
layout: post
title:  "PHP 7 Support"
date:   2016-04-14 20:08:44 +0100
categories: Blog
image: /assets/images/blog/php7.png
excerpt_separator: <!--more-->
---
Joomla 3.5 was released [last week](https://www.joomla.org/announcements/release-news/5654-joomla-3-5-is-here.html). This new version included lots of lovely features, but one which many of our community have asked about is support for PHP7.<!--more--> Joomla now includes support for the recently released PHP7 scripting language, and the aim of this post if to clarify the support for HWDMediaShare. PHP7 was recently announced with [significant performance improvements](https://www.gavick.com/blog/joomla-php-7-speedtest) and is now available for use by the general public. Joomla can run twice as fast and with half the memory usage on systems that run PHP7, so we understand why people are excited about this major new release of PHP.

We can now confirm that HWDMediaShare 2.0.5 is compatible with Joomla 3.5 and PHP7.

## Joomla Performance Tests

There are many articles offering detailed Joomla performance tests for the new PHP7, but we'll do a quick comparison for HWDMediaShare pages. These tests are run on a localhost server using WAMP. The PHP versions which have been compared are **PHP 5.6.16**, and **PHP 7.0.0**. The Joomla page being tested is the HWDMediaShare media view. 

### PHP6

The total load time (afterRender event) was 936.05ms and consumed 15.87MB of memory.

![](/assets/images/blog/content/profile-php6.png)

### PHP7

The total load time (afterRender event) was 505.03ms and consumed 11.65MB of memory.

![](/assets/images/blog/content/profile-php7.png)

## Performance Test Comparisons

<table class="category table table-striped table-bordered table-hover">

<tbody>

<tr>

<td> </td>

<td>PHP 5.6.16</td>

<td>PHP 7.0.0</td>

</tr>

<tr>

<td>Load Time</td>

<td>936.05ms</td>

<td>505.03ms</td>

</tr>

<tr>

<td>Memory Usage</td>

<td>15.87MB</td>

<td>11.65MB</td>

</tr>

</tbody>

</table>

These tests demonstrate that making the switch to PHP7 **reduces the load time by 46% and saves 27% of memory**.
