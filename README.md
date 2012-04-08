PyIndex README File 
-------------------
This is just a simple single process IRC Indexer script written in python.
It can be called by a bash script to run through a predefined list to
gather data from several networks at once hence removing the need for a
multi-threaded indexer all together.

It's released under the GNU General Public License so feel free to modify
it to suit your needs so long as you credit me with the base work.
A copy of the license can be found in the LICENSE file.

USAGE
-----
Just run ./pyindex server.address.here and the script will do the rest.

INDEXER KEY
-----------
The indexer uses a shorthand to minimize the size of the files it generates.
It also uses time() to generate epoch based timestamps.

Generally it's split into either Timestamp:Identifier:Data or Identifier:Data
depending on if a timestamp is required for it or not.

Identifier key:  
NN = The Network's Name  
IT = IRCd Type the Network is using  
LS = Last Server the bot connected to  
TS = Total Servers in the Network  
TC = Total Channels on the Network  
CU = Current Users on the Network  
TU = Total Users on the Network