<img src="assets/selfie.jpeg" style="display: block; width: 40%; margin-left: auto; margin-right: auto;"/>

I'm a CS undergrad at Yale, primarily interested in programming languages and knowledge management. You can find me on [Github](https://github.com/ehatti) and [LinkedIn](https://www.linkedin.com/in/eashan-hatti-777387288). My email is `<first>.<last>@<school>.edu`

{% for post in site.posts %}
  <hr>
  <article style="width: 90%; margin: 0 auto">
    <h3>{{ post.title }} — {{ post.date | date: "%B %-d, %Y" }}</h3>
    {% if post.excerpt %}
      <p>{{ post.excerpt }}</p>
    {% endif %}
    <a href="{{ post.url | relative_url }}">Read more</a>
  </article>
{% endfor %}

---

$$
\frac{
  \Gamma, x : A \vdash e : B
}{
  \Gamma \vdash \lambda x. e : \Pi_{x : A} B
}
$$