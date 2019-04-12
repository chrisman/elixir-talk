<!-- .slide: data-background-image="assets/img/pig.webp" data-background-size="contain" -->
# The Presentation Will Begin Shortly

---

<!-- .slide: data-background-image="assets/img/kanban.png" data-background-size="contain" -->

note: kanban!

---

# Front Endsday

Elixir, Phoenix, Elm

note: make your face friendly

What IS Elixir/Phoenix? Elm?

---

## the plan

2. Credibility <!-- .element: class="fragment" -->

3. Elixir, Phoenix, Elm <!-- .element: class="fragment" -->

---

# Credibility

<i class="fa fa-slack" aria-hidden="true"></i> chrisbrown
<i class="fa fa-twitter" aria-hidden="true"></i> chrismanbrown
<i class="fa fa-github" aria-hidden="true"></i> chrisman

- 💻 developer <!-- .element: class="fragment" -->

- 📿 yoga teacher <!-- .element: class="fragment" -->

note: you are chris brown


<!-- .slide: data-background-image="assets/img/dogs.png" data-background-size="contain" -->


<!-- .slide: data-background-image="assets/img/dohere.gif" data-background-size="contain" -->


<!-- .slide: data-background-image="assets/img/emad.jpg" data-background-size="contain" -->
# Weirdness

note: I haven't used this in production
and Elixir/Phoenix is pretty much BACK end

---

# Web Stacks

| Language   | Web Framework   | Frontend    |
|------------|-----------------|-------------|
| JavaScript | Node.js/Express | HTML/JS/CSS |
| Ruby       | Ruby on Rails   | HTML/JS/CSS |
| Elixir     | Phoenix         | Elm         |


# Virtual Machines

| Language | Compiles to | Virtual Machine      |
|----------|-------------|----------------------|
| Clojure  | Java        | Java Virtual Machine |
| Elixir   | Erlang      | Beam                 |



# Erlang?

- Distributed, Fault-tolerant <!-- .element: class="fragment" -->

- Functional <!-- .element: class="fragment" -->

- Concurrent <!-- .element: class="fragment" -->

- Open Source <!-- .element: class="fragment" -->


# Elixir?

- Friendly <!-- .element: class="fragment" -->

- Functional <!-- .element: class="fragment" -->


# Elixir

| Language   | Dependencies | Config/Build |
|------------|--------------|--------------|
| JavaScript | npm install  | webpack?     |
| Elixir     | mix          | mix          |


# Elixir
(continued)

| Serve   | Migrations |
|---------|------------|
| npm run | knex       |
| mix     | mix        |

note: here comes a gif with lots of mix



<!-- .slide: data-background-image="assets/img/exdoc.gif" data-background-size="contain" -->


# Elixir is (not) like Ruby


<!-- .slide: data-background-image="assets/img/mvc.gif" data-background-size="contain" -->


<!-- .slide: data-background-image="assets/img/router.png" data-background-size="contain" -->

---

# Elm

- Weird  <!-- .element: class="fragment" -->

- Functional  <!-- .element: class="fragment" -->

- Error messages!  <!-- .element: class="fragment" -->


<!-- .slide: data-background-image="assets/img/elm-error-01.png" data-background-size="contain" -->


<!-- .slide: data-background-image="assets/img/elm-error-02.png" data-background-size="contain" -->


<!-- .slide: data-background-image="assets/img/elm-error-03.png" data-background-size="contain" -->


# Architecture

model, view, update


## model

```elm
-- Model

type alias Model =
    Int

model : Model
model =
    0
```


## view

```elm
view : Model -> Html Msg
view model =
    div []
        [ h1 [] [ text "My County Counter!" ]
        , button [ onClick Decrement ] [ text "Decrement" ]
        , span [] [ text (toString model) ]
        , button [ onClick Increment ] [ text "Increment" ]
        , div []
            [ button [ onClick Reset ] [ text "Reset" ] ]
        ]
```


## update

```elm
-- update

type Msg
    = Increment
    | Decrement
    | Reset

update : Msg -> Model -> Model
update msg model =
    case msg of
        Increment ->
            model + 1

        Decrement ->
            model - 1

        Reset ->
            0
```


<!-- .slide: data-background-image="assets/img/why.webp" data-background-size="contain" -->


# Resources

Course

- https://www.udemy.com/the-complete-elixir-and-phoenix-bootcamp-and-tutorial
- https://egghead.io/courses/start-using-elm-to-build-web-applications

Book

- https://learnyousomeerlang.com/

Documentary!

- https://doc.honeypot.io/elixir-documentary-2018/


<!-- .slide: data-background-image="assets/img/bye.gif" data-background-size="contain" -->
# bye!
