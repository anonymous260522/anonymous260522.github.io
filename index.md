---
layout: default
---

## Abstract

Learning to evaluate and improve policies is a core problem of Reinforcement Learning (RL). 
Traditional RL algorithms learn a value function defined for a single policy. 
A recently explored competitive alternative is to learn a single value function for many policies. 
Here we combine the actor-critic architecture of Parameter-Based Value Functions and the policy embedding of Policy Evaluation Networks to learn a single value function for evaluating (and thus helping to improve) any policy represented by a deep neural network (NN). 
The method yields competitive experimental results. 
In continuous control problems with infinitely many states, our value function minimizes its prediction error by simultaneously learning a small set of  `probing states' and a mapping from actions produced in probing states to the policy's return. 
The method extracts crucial abstract knowledge about the environment in form of very few states sufficient to fully specify the behavior of many policies. 
A policy improves solely by changing actions in probing states, following the gradient of the value function's predictions.  
Surprisingly, it is possible to clone the behavior of a near-optimal policy in Swimmer-v3 and Hopper-v3 environments only by knowing how to act in 3 and 5 such learned states, respectively. 
Remarkably, our value function trained to evaluate NN policies is also invariant to changes of the policy architecture: we show that it allows for zero-shot learning of linear policies competitive with the best policy seen during training. 


## Hopper:

{% assign img_size = 95 %}
<img src="/assets/gifs/hopper/videoact_first0.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/hopper/videoact_first1.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/hopper/videoact_first2.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/hopper/videoact_first3.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/hopper/videoact_first4.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">

<img src="/assets/gifs/hopper/videoact_first0.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/hopper/videoact_first1.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/hopper/videoact_first2.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/hopper/videoact_first3.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/hopper/videoact_first4.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">

<img src="/assets/gifs/hopper/videoact_first0.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/hopper/videoact_first1.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/hopper/videoact_first2.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/hopper/videoact_first3.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">
<img src="/assets/gifs/hopper/videoact_first4.gif" width="{{img_size}}" height="{{img_size}}" alt="gif">



There should be whitespace between paragraphs.

There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.

# Header 1

This is a normal paragraph following a header. GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

## Header 2

> This is a blockquote following a header.
>
> When something is important enough, you do it even if the odds are not in your favor.

### Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

#### Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
