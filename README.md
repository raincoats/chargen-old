# chargen

It does what you think it does.

The file `chargen.c` generates chars, `strings-chargen.c` just uses pre generated strings and spews them out (way faster). Check it:

    echo "ten seconds of output"
    ten seconds of output
    
    % ./chargen | pv > /dev/null
    6.42MiB 0:00:10 [ 323KiB/s] [   <=>                                                  ]
    
    % ./strings-chargen | pv > /dev/null
     6.6GiB 0:00:10 [ 670MiB/s] [   <=>                                                  ]


