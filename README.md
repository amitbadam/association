<h1>Simple Association</h1>

rails g scaffold User name:string email:string

rails g scaffold Micropost content:string user_id:integer


app/models/user.rb<br>
has_many :microposts

app/models/micropost.rb<br>
belongs_to :user
