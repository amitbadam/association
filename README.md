Simple Association

rails g scaffold User name:string email:string

rails g scaffold Micropost content:string user_id:integer


app/models/user.rb
has_many :microposts

app/models/micropost.rb
belongs_to :user
