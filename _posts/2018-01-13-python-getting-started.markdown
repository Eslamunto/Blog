---
layout:     post
comments:	true
title:      "REVIEW: Python: Getting Started Course"
subtitle:   "On PluralSight by Bo Milanovich"
date:       2018-01-13 13:12:18
author:     "Eslam Maged"
header-img:	"img/post-bg-04.jpg"
description:	"Course review and notes"
---


<h1><a id="Python_Getting_Started_0"></a>Python: Getting Started</h1>
<h6><a id="By_Bo_Milanovichhttpstwittercompythonbolangen_1"></a>By: <a href="https://twitter.com/pythonbo?lang=en">Bo Milanovich</a></h6>
<h6><a id="Course_Link_PluralSighthttpswwwpluralsightcomcoursespythongettingstarted_2"></a>Course Link: <a href="https://www.pluralsight.com/courses/python-getting-started">PluralSight</a></h6>
<h2><a id="Course_Review_4"></a>Course Review:</h2>
<p>From my little point of view, Bo did such a great job in simplifying the language and making it easy to grasp for absolute beginners. This course is not for you in case you have a background in Python, maybe you can use it to refresh your python skills but I would rather go for a cheat sheet in case you are an experienced developer.<br>
If you are a beginner or someone who is curious about getting introduced to programming and to python, I would absolutely recommend buying the course from PluralSight.</p>
<p>Below are my notes and simple cheat sheet to remember the important things that were mentioned in the course.</p>
<h2><a id="Course_Notes_11"></a>Course Notes</h2>
<h4><a id="What_is_python_13"></a>What is python?</h4>
<p>Python is an interpretted, object-oriented, high level programming language with such a high productivity level.</p>
<h4><a id="Basic_Syntax_17"></a>Basic Syntax:</h4>
<pre><code class="language-sh"><span class="hljs-built_in">print</span> statement
<span class="hljs-built_in">print</span>(<span class="hljs-string">"Hello World!"</span>)
</code></pre>
<h4><a id="Types_in_python_23"></a>Types in python</h4>
<p>Python does not require type declaration for variables unlike Java</p>
<h4><a id="Integers_and_floats_26"></a>Integers and floats</h4>
<ul>
<li>ints can be +ve or -ve but can’t have decimal points</li>
<li>floats can be decimals</li>
<li>python 3 introduces complex number as a type</li>
<li>use the following methods to convert from int to float or the opposite</li>
</ul>
<pre><code class="language-sh">int(<span class="hljs-number">32.5</span>) <span class="hljs-comment"># 32</span>
<span class="hljs-built_in">float</span>(<span class="hljs-number">5</span>)  <span class="hljs-comment"># 5.0</span>
</code></pre>
<h4><a id="Strings_35"></a>Strings</h4>
<ul>
<li>by default they are unicode in python 3</li>
<li>strings can be decalred using single quotes, double quotes or trible quotes (used more for class documentation)</li>
<li>common string methods:</li>
</ul>
<pre><code class="language-sh"><span class="hljs-string">'hello'</span>.capitalize() == <span class="hljs-string">'Hello'</span>
<span class="hljs-string">'hello'</span>.replace(<span class="hljs-string">'e'</span>,<span class="hljs-string">'a'</span>) == <span class="hljs-string">'hallo'</span>
<span class="hljs-string">'hello'</span>.isalpha() == True <span class="hljs-comment"># means that all characters are letters</span>
<span class="hljs-string">'123'</span>.isdigit() == True <span class="hljs-comment"># means that all characters are digits</span>
</code></pre>
<ul>
<li>to splits a string into a list</li>
</ul>
<pre><code class="language-sh"><span class="hljs-string">"some,csv,values"</span>.split(<span class="hljs-string">","</span>) == [<span class="hljs-string">"some"</span>, <span class="hljs-string">"csv"</span>, <span class="hljs-string">"values"</span>]
</code></pre>
<ul>
<li>String format function</li>
</ul>
<pre><code class="language-sh">name = <span class="hljs-string">"Eslam"</span>
machine = <span class="hljs-string">"Lenovo"</span>
<span class="hljs-string">"Nice to meet you {0}. I am {1}"</span>.format(name, machine)
</code></pre>
<ul>
<li>Starting in python 3.6, you can do the following:</li>
</ul>
<pre><code class="language-sh">f<span class="hljs-string">"Nice to meet you {name}. I am {machine}"</span>
</code></pre>
<h4><a id="Boolean_and_None_60"></a>Boolean and None</h4>
<pre><code class="language-sh">var1 = True
var2 = False
aliens_found = None <span class="hljs-comment">#None is simillar to null in different languages</span>
</code></pre>
<h4><a id="If_statements_67"></a>If statements</h4>
<pre><code class="language-sh">number = <span class="hljs-number">6</span>
<span class="hljs-keyword">if</span> number == <span class="hljs-number">6</span>:
    <span class="hljs-built_in">print</span>(<span class="hljs-string">"Number is 6"</span>)
<span class="hljs-keyword">else</span>:
    <span class="hljs-built_in">print</span>(<span class="hljs-string">"Number is NOT 6"</span>)
</code></pre>
<ul>
<li>we use the keyword <strong>is</strong> to see if two variables are pointing to the same object in memory</li>
</ul>
<h4><a id="Truthy_and_Falsy_values_77"></a>Truthy and Falsy values</h4>
<p>python checks if  a variable has a truthy value, a truthy value in integers is anything which is not zero or a string that contains any text.<br>
This is useful in case of lists, where you do not need to check for list size as in other programming languages put you would rather do the following</p>
<pre><code class="language-sh"><span class="hljs-keyword">if</span> student_list:
    execute some code <span class="hljs-keyword">if</span> list exists
<span class="hljs-keyword">if</span> not
!=
is not
</code></pre>
<h4><a id="Multiple_if_statements_88"></a>Multiple if statements</h4>
<pre><code class="language-sh">and, or
<span class="hljs-keyword">if</span> x and y:
<span class="hljs-keyword">if</span> x or y:
</code></pre>
<h4><a id="Ternary_if_statements_95"></a>Ternary if statements</h4>
<pre><code class="language-sh">a=<span class="hljs-number">1</span>
b=<span class="hljs-number">2</span>
<span class="hljs-string">"bigger"</span> <span class="hljs-keyword">if</span> a &gt; b <span class="hljs-keyword">else</span> <span class="hljs-string">"smaller"</span>
</code></pre>
<h4><a id="Lists_102"></a>Lists</h4>
<ul>
<li>to create an empty list just use the square brakcets</li>
</ul>
<pre><code class="language-sh">student_names = []
</code></pre>
<ul>
<li>a list that has some elements</li>
</ul>
<pre><code class="language-sh">student_names = [<span class="hljs-string">"Eslam"</span>, <span class="hljs-string">"Maged"</span>, <span class="hljs-string">"Ahmed"</span>]
</code></pre>
<ul>
<li>to access an item in the list</li>
</ul>
<pre><code class="language-sh">student_names[<span class="hljs-number">0</span>]
student_names[-<span class="hljs-number">1</span>] == <span class="hljs-string">"Ahmed"</span>
</code></pre>
<ul>
<li>Add new items to a list</li>
</ul>
<pre><code class="language-sh">student_list.append(<span class="hljs-string">"Hoba"</span>) <span class="hljs-comment"># add to the end</span>
</code></pre>
<ul>
<li>to check if an element is in the list</li>
</ul>
<pre><code class="language-sh"><span class="hljs-string">"Hoba"</span> <span class="hljs-keyword">in</span> student_names == True
</code></pre>
<ul>
<li>Number of elements in a list</li>
</ul>
<pre><code class="language-sh">len(student_names) == <span class="hljs-number">4</span> 
</code></pre>
<p>-having multiple types in a list is not a problem. A list can contain different types from different lists</p>
<ul>
<li>to delete an element from a list</li>
</ul>
<pre><code class="language-sh">del student_names[<span class="hljs-number">2</span>] <span class="hljs-comment"># "Ahmed is not longer in the list"</span>
</code></pre>
<ul>
<li>elements will shift to the left after the delete operation</li>
</ul>
<h4><a id="List_slicing_137"></a>List slicing</h4>
<ul>
<li>if we want to ignore the first element in the list and get the rest of the list</li>
</ul>
<pre><code class="language-sh">student_names[<span class="hljs-number">1</span>:] == [<span class="hljs-string">'Maged'</span>, <span class="hljs-string">'Ahmed'</span>] 
student_names[<span class="hljs-number">1</span>:-<span class="hljs-number">1</span>] == [<span class="hljs-string">'Maged'</span>] <span class="hljs-comment"># we have ignored the first item and the last item in the list</span>
</code></pre>
<h4><a id="For_Loop_144"></a>For Loop</h4>
<pre><code class="language-sh"><span class="hljs-keyword">for</span> student <span class="hljs-keyword">in</span> student_names:
    <span class="hljs-built_in">print</span>(student)
</code></pre>
<h4><a id="range_150"></a>range</h4>
<pre><code class="language-sh">x = <span class="hljs-number">0</span>
<span class="hljs-keyword">for</span> x <span class="hljs-keyword">in</span> range(<span class="hljs-number">10</span>): <span class="hljs-comment"># code executes from 0 till 10</span>
range(<span class="hljs-number">5</span>,<span class="hljs-number">10</span>) <span class="hljs-comment"># 5,6,7,8,9</span>
range(<span class="hljs-number">4</span>,<span class="hljs-number">10</span>,<span class="hljs-number">2</span>) <span class="hljs-comment"># 4,6,8</span>
</code></pre>
<h4><a id="Break_and_continue_158"></a>Break and continue</h4>
<ul>
<li>break is used to get out of the loop in case you got what you want</li>
<li>continue is used to skip an iteration without breaking the loop</li>
</ul>
<h4><a id="Dictionary_162"></a>Dictionary</h4>
<ul>
<li>In python dictionary we have keys and values</li>
</ul>
<pre><code class="language-sh">student = {
    <span class="hljs-string">"name"</span>: <span class="hljs-string">"Eslam"</span>,
    <span class="hljs-string">"id"</span>: <span class="hljs-string">"25"</span>,
    <span class="hljs-string">"feedback"</span>: None
}
</code></pre>
<h4><a id="to_retreive_data_from_dictionary_171"></a>to retreive data from dictionary</h4>
<pre><code class="language-sh">student[<span class="hljs-string">"name"</span>] == <span class="hljs-string">"Eslam"</span>
student[<span class="hljs-string">"last_name"</span>] == KeyError
</code></pre>
<ul>
<li>in case you want to query a key and you are not sure that it exists there then you should add a fallback</li>
</ul>
<pre><code class="language-sh">student.get[<span class="hljs-string">"last_name"</span>, <span class="hljs-string">"unknown"</span>] == <span class="hljs-string">"unknown"</span> <span class="hljs-comment">#True</span>
</code></pre>
<ul>
<li>to get all keys in a dictionary</li>
</ul>
<pre><code class="language-sh">student.keys() =&gt; returns a list of all keys
student.values() =&gt; returns a list of all values
</code></pre>
<h4><a id="Exceptions_188"></a>Exceptions</h4>
<ul>
<li>events that occur during the execution of your program that causes problems while executing.</li>
</ul>
<pre><code class="language-sh">try:
    last_name = student[<span class="hljs-string">"last_name"</span>]
    numbered_last_name = last_name + <span class="hljs-number">3</span>
except KeyError:
    <span class="hljs-built_in">print</span>(<span class="hljs-string">"Error finding last name"</span>)
except TypeError as error:
    <span class="hljs-built_in">print</span>(<span class="hljs-string">"cant add two values"</span>)
    <span class="hljs-built_in">print</span>(error) <span class="hljs-comment">#used to show the error in the logs</span>
</code></pre>
<h4><a id="Other_data_types_202"></a>Other data types</h4>
<pre><code class="language-sh">complex
long <span class="hljs-comment">#only in python2</span>
bytes and bytearray
tuple = (<span class="hljs-number">3</span>,<span class="hljs-number">5</span>,<span class="hljs-number">1</span>,<span class="hljs-string">"Mark"</span>)
<span class="hljs-built_in">set</span> and frozenset
<span class="hljs-built_in">set</span>([<span class="hljs-number">3</span>,<span class="hljs-number">2</span>,<span class="hljs-number">1</span>,<span class="hljs-number">5</span>]) == (<span class="hljs-number">1</span>,<span class="hljs-number">2</span>,<span class="hljs-number">3</span>,<span class="hljs-number">5</span>)
</code></pre>
<h4><a id="Function_212"></a>Function</h4>
<pre><code class="language-sh">def <span class="hljs-keyword">function</span>_name(input_params):
    <span class="hljs-keyword">function</span>_body
    <span class="hljs-built_in">return</span> <span class="hljs-built_in">return</span>_value
</code></pre>
<ul>
<li>multiple arguments for a function we use *args</li>
</ul>
<pre><code class="language-sh">def var_args(name, *args):
    <span class="hljs-built_in">print</span>(name)
    <span class="hljs-built_in">print</span>(args) <span class="hljs-comment">#refet to args inside function body we do not use the astrics </span>
var_args(<span class="hljs-string">"Eslam"</span>, <span class="hljs-string">"love pythong"</span>, None, <span class="hljs-number">77</span>, True)
</code></pre>
<ul>
<li>It would be better to have names to the arguments instead of having to loop through all the given arguments to extract the needed variable/value; that’s where we use kwargs…</li>
</ul>
<pre><code class="language-sh">def var_args(name, **kwargs):
    <span class="hljs-built_in">print</span>(name)
    <span class="hljs-built_in">print</span>(kwargs[<span class="hljs-string">"description"</span>], kwargs[<span class="hljs-string">"feedback"</span>])
var_args(<span class="hljs-string">"Eslam"</span>, description=<span class="hljs-string">"love pythong"</span>, feedback=None, subscriber=True)
</code></pre>
<h4><a id="Input_233"></a>Input</h4>
<ul>
<li>to take input from the user we use the input method</li>
</ul>
<pre><code class="language-sh">student_name = input(<span class="hljs-string">"Enter student name"</span>)
</code></pre>
<h4><a id="Nested_Function_239"></a>Nested Function</h4>
<ul>
<li>sometimes you need to add a function to do a job inside another function thats where we use neste functions and call it from the outer function. The nested function has access to the variables defined in the outer function. This is called a closure</li>
</ul>
<pre><code class="language-sh">def get_student():
    students = [<span class="hljs-string">"eslam"</span>, <span class="hljs-string">"maged"</span>]
    def get_Students_titlecase():
        <span class="hljs-keyword">for</span> student <span class="hljs-keyword">in</span> students:
            students_titlecase.append(student.title())
        <span class="hljs-built_in">return</span> student_titlecase
    students_titlecase_names = get_students_titlecase()
    <span class="hljs-built_in">print</span>(students_titlecase_names)
</code></pre>
<h4><a id="Working_with_files_252"></a>Working with files</h4>
<pre><code class="language-sh">try:
    f = open(<span class="hljs-string">"stuents.txt"</span>, <span class="hljs-string">"r"</span>)
    <span class="hljs-keyword">for</span> student <span class="hljs-keyword">in</span> f.readlines():
        add_student(student)
    f.close()
except Exception:
    <span class="hljs-built_in">print</span>(<span class="hljs-string">"could not read file"</span>)
</code></pre>
<h4><a id="Access_modes_in_python_263"></a>Access modes in python</h4>
<pre><code class="language-sh"><span class="hljs-string">"w"</span> - writing: overwrites the entire file
<span class="hljs-string">"r"</span> - reading a text file
<span class="hljs-string">"a"</span> = appending to a new or existing file
<span class="hljs-string">"rb"</span> - reading a binary file
<span class="hljs-string">"wb"</span> - writing to a binary file
</code></pre>
<h4><a id="Classes_272"></a>Classes</h4>
<ul>
<li>class is a logical group of functions and data. functions in a class are called methods</li>
<li>classes allow you to write more readable and more maintable code.</li>
<li>class is a blueprint/building block and the instances of the class are the actualy blocks</li>
</ul>
<pre><code class="language-sh">class Student:
    pass
</code></pre>
<ul>
<li>to initiate a new instance of a class</li>
</ul>
<pre><code class="language-sh">student = Student()
</code></pre>
<h5><a id="Class_example_with_a_function_285"></a>Class example with a function</h5>
<pre><code class="language-sh">students = []
class Student:
    def add_student(self, name, student_id=<span class="hljs-number">332</span>):
        student = {<span class="hljs-string">"name"</span>: name, <span class="hljs-string">"student_id"</span>: student_id}
        students.append(student)

student = Student()
student.add_student(<span class="hljs-string">"Mark"</span>)
</code></pre>
<ul>
<li>The constructor method is a special method in python classes that gets executed everytime you create a new isntance of that class</li>
<li>Constructor method in python has the syntax of init</li>
</ul>
<pre><code class="language-sh">def __init__(self, name, student_id):
    pass
</code></pre>
<ul>
<li>To print an instance of a class we use the method override _ <em>str</em> _</li>
</ul>
<pre><code class="language-sh">def __str__(self):
    <span class="hljs-built_in">return</span> <span class="hljs-string">"student"</span> <span class="hljs-comment">#prints student when trying to print the object otherwise we would get a memory reference</span>
</code></pre>
<h4><a id="Inheritance_308"></a>Inheritance</h4>
<pre><code class="language-sh">class HighSchoolStudent(Student):
<span class="hljs-comment"># we can override   methods and variables in the parent class</span>
</code></pre>
<h4><a id="calling_a_parent_method_in_the_inherited_class_313"></a>calling a parent method in the inherited class</h4>
<pre><code class="language-sh">def get_name_capitalized(self):
    original_value = super().get_name_capitalized()
</code></pre>
<ul>
<li>
<p>In python you can inherit from multiple classes</p>
</li>
<li>
<p>In python there is a convention to put an underscore before the method name to state that the method should not be overriden or even used directly. There are no interfaces in python</p>
</li>
<li>
<p>pyInstaller to generate executable files from the python program you wrote</p>
</li>
</ul>


<div id="disqus_thread"></div>
<script>
    /**
     *  RECOMMENDED CONFIGURATION VARIABLES: EDIT AND UNCOMMENT THE SECTION BELOW TO INSERT DYNAMIC VALUES FROM YOUR PLATFORM OR CMS.
     *  LEARN WHY DEFINING THESE VARIABLES IS IMPORTANT: https://disqus.com/admin/universalcode/#configuration-variables
     */
    /*
    var disqus_config = function () {
        this.page.url = PAGE_URL;  // Replace PAGE_URL with your page's canonical URL variable
        this.page.identifier = PAGE_IDENTIFIER; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
    };
    */
    (function() {  // DON'T EDIT BELOW THIS LINE
        var d = document, s = d.createElement('script');
        
        s.src = 'https://eslamaged.disqus.com/embed.js';
        
        s.setAttribute('data-timestamp', +new Date());
        (d.head || d.body).appendChild(s);
    })();
</script>
<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript" rel="nofollow">comments powered by Disqus.</a></noscript>