
How we make columns using our custom framework

we have a custom boilerplater, and we use emoji's for some CSS classes
they make it not only more fun, but also easier to see at a glance what our code is doing
the 5 classes you need to understand right away are as follows:

    👪 is flexbox
    🔲 is max-width
    📚 is display:block on smaller screens 
    🙎‍♂️ is max width 
    🙎‍♀️ is min width

these css classes are what we use to quickly create columns
for example, the following code will create 3 equal columns, that will stack vertically on screens under 1000 pixels

    <div class="🔲1200 👪 📚1000">
        <div class="🙎‍♂️33 🙎‍♀️33">
            <p>First Column</p>
        </div>
        <div class="🙎‍♂️33 🙎‍♀️33">
            <p>Second Column</p>
        </div>
        <div class="🙎‍♂️33 🙎‍♀️33">
            <p>Third Column</p>
        </div>
    </div>

if you read the boilerplate stylesheet, you can quickly see that these classes simply make use of flexbox
the problem has always been that flexbox can be confusing to write, and even more confusing to read

one other note
the numbers, like 📚1000, are predefined in the boilerplate
read boilerplate.css to see what is available to you
we can add more as needed, but don't bother for this project. 