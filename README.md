<h1>Simple Association</h1>

<h6>rails g scaffold User name:string email:string</h6>

<h6>rails g scaffold Micropost content:string user_id:integer</h6>


<h6>app/models/user.rb</h6><br>
has_many :microposts

<h6>app/models/micropost.rb</h6><br>
belongs_to :user
