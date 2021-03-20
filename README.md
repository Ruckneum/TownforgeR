# TownforgeR
An R-package for interacting with the Townforge blockchain

Read more about Townforge at: www.townforge.net

Townforge is a blockchain based game forked originally from the Monero project (https://github.com/monero-project).
This is a package written for the R statistical software language, for curl'ing the Townforge RPC commands and interacting with the daemon. 
TownforgeR parses the input JSON according to the web app, and the returned JSON into R-compatible lists and data frames.

It comes with an R Shiny interface, i.e. a graphical web browser, in addition to the base R functionality.

Some example TownforgeR code run in a base R terminal and launching the built web app:


\> library(TownforgeR)

\> TownforgeR::tf_rpc_curl(method="get_block_count") # Curl the RPC with the method "get_block_count", assuming URL to be 127.0.0.1:18881

\> TownforgeR::shinyTF() # Launch the R Shiny interface in the default browser
