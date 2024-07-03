# Gadgets

List of our gadgets...

{% set imgNameList = generateTemplateImgNameList() %}

{% for imgPath, name, path in imgNameList %}
![Gadget Image]({{ imgPath }})
[{{ name }}]({{ path }})
{% endfor %}
