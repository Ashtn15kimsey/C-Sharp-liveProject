# C-Sharp-liveProject

The last two weeks a group of students and I were tasked with to develope Web Application built using ASP .Net MVC and Entity Framework. The project is a website that is interactive and user friendly.I largely worked on the front end of the website creating the edit, create page as well as styling them. I also created a blogPost where users had the option to create a blog post and had the choice to update, delete, edit, and create a new blog. Working on this project with my peers gave me the confidence to take on any task no matter how large or difficult it may be. Learning from trial and error is much better than  quitting for me.Over the last two weeks I gained new knowledge and experience working with others to accoplish a task that I will for sure use in the future.

Below are some of the projects I worked on for our Theatre website.I created a Entity Model for a Blog Post for users to create, edit,and write a blog.
using System;
using System.Collections.Generic;
using System.Linq;
using System.Web;
using System.IO;

namespace TheatreCMS3.Areas.Blog.Models
{

    public class BlogPostModel
    {
        public int ID { get; set; }
        public string Title { get; set; }
        public string Content { get; set; }
        public DateTime Posted { get; set; }
        public string Author { get; set; }
    }
I also created a class called Postmaster which determines if the users blog is rejected or pending to post.
using System;
using System.Collections.Generic;
using System.Linq;
using System.Web;
using TheatreCMS3.Models;

namespace TheatreCMS3.Areas.Blog.Models
{
    public class Postmaster : ApplicationUser
    {
        public static int PublishedBlogPosts;
        public static int RejectedBlogPosts;
        public static int PendingPosts;


    }
}

I worked on some front end projects also making the the website more color coordianted and follwing a specific color schema.
.submit-btn{
    border:none;
    color: white;
    background-color: red;
    text-align:center;
    padding: 10px 24px;
    border: 2px solid red;

}
.backtoList{
    background-color: red;
    color:white;
    text-align: center;
    padding: 10px 24px;
    border: 2px solid red;

}
.create-form{
background-color:red;
color: white;
border: 4px solid red;
border-radius: 30px;
}
.edit-form{
color:white;
background-color: red;
border: 5px solid red;
border-radius: 25px;
}

