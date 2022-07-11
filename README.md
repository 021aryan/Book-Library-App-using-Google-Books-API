# Book-Library-App-using-Google-Books-API
Book Library App using Google Books API.
If you are looking for building a book library app and you want to load a huge data of books then for adding this feature,
you have to use a simple API which is provided by Google, and of course, it’s free.
In this article, we will take a look at the implementation of this API in our Android App. 

What we are going to build in this article? 
We will be building a simple application in which we will be searching different types of books and we will
get to see the list of books related to that topic in our RecyclerView. For searching these books we will be
using a free API provided by Google which holds a huge collection of books. A sample video is given below to 
get an idea about what we are going to do in this article. Note that we are going to implement this project using
the Java language.
Step by Step Implementation
Step 1: Create a New Project

To create a new project in Android Studio please refer to How to Create/Start a New Project in Android Studio. Note that select Java as the programming language.

Step 2: Add the dependency for Volley in your Gradle files
Navigate to the app > Gradle Scripts > build.gradle file and add below dependency in the dependencies section. 

implementation ‘com.android.volley:volley:1.1.1’

implementation ‘com.squareup.picasso:picasso:2.71828’ 

After adding the below dependencies in your gradle file now sync your project and now we will move towards our activity_main.xml file. As we will be using volley to fetch data from our API and Picasso image loading library to load images from URL.   

Step 3: Adding permissions for the Internet 

Navigate to the app > AndroidManifest.xml and add the below permissions to it. 
