# CRUD_cheat_sheet

## Routes

Methode ressources taken one parameters and create all the routes automatically.

```ruby
ressources :photos
```

to create the path, just take the prefix (left column accessible using command)

```ruby
rails routes
```

## View

then in the view > index.html.erb add the mention _path to the prefix. To access a particular article, you can also pass the variable "id"

```ruby
photo_path(post.id)
```

## Controller

In order to display the post, you should create a method show

```ruby
def show
  @post = Post.find(params: id)
def
```

## view

The in the views folder, you need to create an erb file: show.html.erb

```ruby
<h1> <%= @post.name %>

<p>
  <a href = <%= "posts_path class" = btn btn-primary%>Revenir aux articles</a>
</p>

```
## Create forms in rails 

To facilitate the form creation, go to https://guides.rubyonrails.org/form_helpers.html
