

Create structure:

```
<!DOCTYPE html>
<html>

<body>
</body>

</html>
```


Add header:

```diff
<!DOCTYPE html>
<html>

<body>
+    <h1>Years to Days calculator</h1>
</body>

</html>

```

Add input and button:

```diff
<!DOCTYPE html>
<html>

<body>
    <h1>Years to Days calculator</h1>

+    Please enter your age in years:
+    <input id="myage" type="number">
+    <button>Calculate</button>
</body>

</html>
```


Add `<script>` with a dummy function, then call the function when clicking the button.

```diff
<!DOCTYPE html>
<html>

<body>
    <h1>Years to Days calculator</h1>

    Please enter your age in years:
    <input id="myage" type="number">
+    <button onclick="calculate();">Calculate!</button>

+    <script>
+        var i = 1;
+        function calculate() {
+            console.log(i++)
+        }
+    </script>
</body>

</html>
```

Replace the dummy function with the aged entered in the form.

```diff
<!DOCTYPE html>
<html>

<body>
    <h1>Years to Days calculator</h1>

    Please enter your age in years:
    <input id="myage" type="number">
    <button onclick="calculate();">Calculate!</button>

    <script>
        var myage;
        function calculate() {
+            myage = document.getElementById("myage").value
+            alert(myage)
        }
    </script>
</body>

</html>
```

Replace the alert with the calculation.

```diff
<!DOCTYPE html>
<html>

<body>
    <h1>Years to Days calculator</h1>

    Please enter your age in years:
    <input id="myage" type="number">
    <button onclick="calculate();">Calculate!</button>

    <script>
        var myage;
        function calculate() {
            myage = document.getElementById("myage").value
+            var myage_days = myage*365
+            alert("You are "+myage_days+" days old")
        }
    </script>
</body>

</html>

```

