
This is a generalized project root skeleton and skeleton generator.

To activate this root in a bash shell:

    . bin/activate

Then, using this package root, you can replicate the current package
root:

    cd ~
    mkroot foo
    cd foo

Or, if you have an existing root that you want to bless with
activatability and replicability:

    cd ~/foo
    mkroot

Then, you can configure that package root with whatever directories
you want to activate by editing its copy of `package.conf`.

    activate PATH bin
    activate LDPATH lib
    activate PYTHONPATH lib/py
    activate RUBY_PATH lib/rb
    activate NODE_PATH lib/js

Then you can activate your new root:

    . bin/activate

`package.conf` is a shell script that's executed in its own directory,
so you can continue to do other shell script things in there.

You can use this tool to create template roots.  Once a root has been
activated, the mkroot command will replicate the currently activated
prototype.

