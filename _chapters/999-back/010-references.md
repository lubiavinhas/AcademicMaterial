---
title: References
slug: references
disable_toc: true
#class: references
---



### Citations in text

Here's an example citation to be included in a text, 
with a link to the references chapter:

```
[(Berg, 1997)](references.html#berg-1997)
```

...which renders as [(Berg, 1997)](references.html#berg-1997).

### Reference list

Use a "references" chapter in the book's end matter to list all of the complete citations,
and receive inbound links from the in-text citations.

To use a "hanging indent" citation style like APA,
either set `class: references` in the front matter of the references page,
or wrap them in a div like this directly in the markdown:

{% raw %}
```html
<div class="references" markdown="block">
```
{% endraw %}

In order to make inbound anchor links from in-text citations work,
we have to include a link in each reference (like the ISBN link below),
and assign it an `id` attribute with `{:#my-id}`.

{% raw %}
```
Berg, C. (1997). *Mastering Guitar Technique: Process and Essence (Classic Guitar).* Mel Bay Publications, Inc.
[ISBN 978-1-610-65058-8](https://en.wikipedia.org/wiki/Special:BookSources?isbn=978-1-610-65058-8){:#berg-1997}.
```
{% endraw %}

...which renders as below.

<div class="references" markdown="block">

## References

Camara, G; Monteiro, A. M. V.; Fucks, S. D.; Carvalho, M. S. (2000) *Spatial Analysis and GIS: A Primer*. [https://www.dpi.inpe.br/gilberto/tutorials/spatial_analysis/spatial_analysis_primer.pdf](https://www.dpi.inpe.br/gilberto/tutorials/spatial_analysis/spatial_analysis_primer.pdf){:#Camara-2000}.

Dangermond, J; Goodchild, M. F. (2020) *Building geospatial infrastructure*, Geo-spatial Information Science, 23:1, 1-9, [DOI: 10.1080/10095020.2019.1698274](https://doi.org/10.1080/10095020.2019.1698274){:#Dangermond-2020}.

Steineger, S.; Hunter, A. J. S.(2012) *The 2012 free and open source GIS software map–A guide to facilitate research, development, and adoption*. [https://doi.org/10.1016/j.compenvurbsys.2012.10.003](https://doi.org/10.1016/j.compenvurbsys.2012.10.003){:#Steineger-2012}.

Waters, N. (2017) *GIS: History*, In book: The International Encyclopedia of Geography. [DOI: 10.1002/9781118786352.wbieg0841](http://dx.doi.org/10.1002/9781118786352.wbieg0841) {:#Waters-2017}
...
</div>

---
```
This file is located at: {{ page.path }}
```
---
