# Laravel-One-to-Many-Polymorphic-Relationship

+ Retrieve Records:

$post = Post::find(1);	 
dd($post->comments);

$video = Video::find(1);	 
dd($video->comments);

------------------------------------------------

+ Create Records:

$post = Post::find(1);	
$comment = new Comment;
$comment->body = "Hi ItSolutionStuff.com";
$post->comments()->save($comment);

$video = Video::find(1);	
$comment = new Comment;
$comment->body = "Hi ItSolutionStuff.com";
$video->comments()->save($comment);	

