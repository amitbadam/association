<h1>Simple Association</h1>

<b>rails g scaffold User name:string email:string</b>

<b>rails g scaffold Micropost content:string user_id:integer</b>


<b>app/models/user.rb</b><br>
has_many :microposts

<b>app/models/micropost.rb</b><br>
belongs_to :user
