---
title: Rancher API - environmentUpgrade
layout: rancher-api-default-v1.0
version: v1.0
lang: en
---

## EnvironmentUpgrade



### Resource Fields

#### Writeable Fields

Field | Type | Create | Update | Default | Notes
---|---|---|---|---|---
dockerCompose | string | Optional | - | - | 
environment | map[string] | Optional | - | - | 
externalId | string | Optional | - | - | 
rancherCompose | string | Optional | - | - | 



<br>

Please read more about the [common resource fields]({{site.baseurl}}/rancher/{{page.version}}/{{page.lang}}/api/common/). These fields are read only and applicable to almost every resource. We have segregated them from the list above.

### Operations
{::options parse_block_html="true" /}
<a id="create"></a>
<div class="action"><span class="header">Create<span class="headerright">POST:  <code>/v1/environmentUpgrades</code></span></span>
<div class="action-contents"> {% highlight json %}
curl -u "${RANCHER_ACCESS_KEY}:${RANCHER_SECRET_KEY}" \
-X POST \
-H 'Content-Type: application/json' \
-d '{
	"dockerCompose": "string",
	"environment": {
		"key": "value-pairs"
	},
	"externalId": "string",
	"rancherCompose": "string"
}' 'http://${RANCHER_URL}:8080/v1/environmentUpgrades'
{% endhighlight %}
</div></div>



