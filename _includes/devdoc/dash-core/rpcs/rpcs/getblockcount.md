{% comment %}
This file is licensed under the MIT License (MIT) available on
http://opensource.org/licenses/MIT.
{% endcomment %}
{% assign filename="_includes/devdoc/dash-core/rpcs/rpcs/getblockcount.md" %}

##### GetBlockCount
{% include helpers/subhead-links.md %}

{% assign summary_getBlockCount="returns the number of blocks in the local best block chain." %}

{% autocrossref %}

The `getblockcount` RPC {{summary_getBlockCount}}

*Parameters: none*

*Result---the number of blocks in the local best block chain*

{% itemplate ntpd1 %}
- n: "`result`"
  t: "number (int)"
  p: "Required<br>(exactly 1)"
  d: "The number of blocks in the local best block chain.  For a new node with only the hardcoded genesis block, this number will be 0"

{% enditemplate %}

*Example from Dash Core 0.12.2*

{% highlight bash %}
dash-cli -testnet getblockcount
{% endhighlight %}

Result:

{% highlight text %}
4627
{% endhighlight %}

*See also*

* [GetBlockHash][rpc getblockhash]: {{summary_getBlockHash}}
* [GetBlock][rpc getblock]: {{summary_getBlock}}

{% endautocrossref %}
