# CommonMark sample document

## Basic inline formatting

Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam **nonumy
eirmod tempor invidunt** ut labore et *dolore magna aliquyam erat*, sed diam
voluptua. `At vero eos et` accusam et

## Headers

### Level 3

#### Level 4

##### Level 5

###### Level 6

## [Links]

Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod
tempor invidunt ut labore et dolore magna aliquyam erat
(<http://www.example.com/autolink>), sed diam voluptua.

Lorem ipsum dolor sit amet, [consetetur
sadipscing](http://www.example.com/inline) elitr, sed diam nonumy eirmod tempor
invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos
et accusam et [justo duo dolores][1] et ea rebum. Stet clita kasd gubergren, no
sea [takimata sanctus](./showcase.md) est Lorem ipsum dolor sit amet.

Ask to <user@example.com>.

[1]: http://www.example.com/reference

## [Images]

Images as blocks:

![The Rust logo](./rust-logo-128x128.png)

## Lists

Unordered lists:

* Lorem impsum
    * Nested
    * Inline
    * Text
* dolor sit amet
    * Nested

    * With Paragraphs and nested blocks:

      > A quote

      And some text at the end
* consetetur sadipscing elitr

Ordered lists:

1. Lorem impsum
    1. Nested
    2. Inline
    3. Text
2. dolor sit amet
    1. Nested

    2. With 
       Paragraphs and nested blocks:

       > A quote

       And some text at the end
3. consetetur sadipscing elitr

And a mix of both:

* Lorem impsum
    1. Nested
    2. Inline
        * With
        * Some
        * Nested
        * Bullets
    3. Text
* dolor sit amet

## Block level elements

Block quotes

> Lorem ipsum dolor sit amet, *consetetur sadipscing elitr*, sed diam nonumy
> eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam
> voluptua.
>
> Lorem ipsum dolor sit amet, **consetetur sadipscing elitr**, sed diam nonumy
> eirmod tempor invidunt ut `labore et dolore magna` aliquyam erat, sed diam
> voluptua.

Before we continue, have a ruler:

----

Code blocks without syntax highlighting:

```
Some plain
code block
   fooo
```

Or with syntax highlighting, eg, Rust:

```rust
fn main() {
    println!("Hello world")
}
```

Or Haskell:

```haskell
main :: IO ()
main = putStrLn "Hello World"
```

Or Scala:

```scala
object HelloWorld {
  def main(args: Array[String]): Unit = {
    println("Hello, world!")
  }
}
```

Or raw codeblocks:

````
```bash
echo 'hi from the innner codeblock'
```
````

## HTML

We can have block html:

<div class="hero">
<p>
Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod
tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At
vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren,
no sea takimata sanctus est Lorem ipsum dolor sit amet.
</p>
</div>

Or inline HTML, as in this paragraph: Lorem ipsum dolor sit amet, consetetur
sadipscing elitr, sed <abbr>diam</abbr> nonumy eirmod tempor invidunt ut labore
et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et
justo duo dolores et ea rebum. <strong>Stet clita kasd gubergren</strong>, no
sea takimata sanctus est Lorem ipsum dolor sit amet.

## Escapes

We now support escaping special characters, such as in \_\_init\_\_.py and in formulas
like \\( \int x dx = \frac{x^2}{2} + C \\).

What about \*this\* or \*\*that\*\*?

\# heading?

\[disabled inline link](target)

\[disabled named link]: target

[named-link][enabled]

[enabled]: bah

\[disabled named link]\[disabled]

[disabled]: bah

|table|
\|-----|

\`code`

] a closing bracket does nothing

\<html>

\> inline code blocks

In code blocks, there will be no escaping:

````
A raw block inside
```
foo
```

* | < > # 
````

[Links]: http://www.example.com/shortcut
[Images]: http://www.example.com/another_shortcut