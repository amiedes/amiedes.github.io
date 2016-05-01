---
layout: post
title: Code snippet
published: true
tags: software, other
---

Esto es un ejemplo de bloque de código:

{% highlight ruby %}
def show
  @widget = Widget(params[:id])
  respond_to do |format|
    format.html # show.html.erb
    format.json { render json: @widget }
  end
end
{% endhighlight %}

Este es el mismo ejemplo pero con la sintaxis de .md:

```ruby
def show
  @widget = Widget(params[:id])
  respond_to do |format|
    format.html # show.html.erb
    format.json { render json: @widget }
  end
end
```

Para mostrar los números de línea:

{% highlight c linenos %}
int main(void) {
    while(1) fork();
}
{% endhighlight %}
