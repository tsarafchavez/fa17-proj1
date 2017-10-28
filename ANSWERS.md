# Q0: Why is this error being thrown?
Needs a pokemon model to create a pokemon (else @pokemon is left uninitized.

# Q1: How are the random Pokemon appearing? What is the common factor between all the possible Pokemon that appear? *
pokemon are being pulled from  seed sample defined in seeds.rb.
 The common factor between the pokemon is that the pokemon dont have a trainer
 
# Question 2a: What does the following line do "<%= button_to "Throw a Pokeball!", capture_path(id: @pokemon), :class => "button medium", :method => :patch %>"? Be specific about what "capture_path(id: @pokemon)" is doing. If you're having trouble, look at the Help section in the README.
the line calls a method that takes in the id of the current pokemon displayed on the screen and passes it to the capture method in the pokemon controller which sets the trainer_id of the pokemon to the id of the current player who is logged in
# Question 3: What would you name your own Pokemon?
I would name it Kanye West because I love kanye. 
# Question 4: What did you pass into the redirect_to? If it is a path, what did that path need? If it is not a path, why is it okay not to have a path here?
I passed  path to redirect_to. 
the path I passed needed the id of the trainer who that pokemon belonged to, since the pokemon you're damaging is not going to belong to the current_trainer (also each user has their own id.)
# Question 5: Explain how putting this line "flash[:error] = @pokemon.errors.full_messages.to_sentence" shows error messages on your form.
in application.html.erb at the end it renders layouts/_messages.html.erb which defines a method to show an error pop up on the screen. The error can be exited (or clicked away).
# Give us feedback on the project and decal below!
it was fun and interactive!

# Extra credit: Link your Heroku deployed app
