1. Transferring the file from cleantax format to rcc uber-mir format
If the input file is in CleanTax file format, need to run "cleantax2rcc.py" first to transfer it to uber-mir format.
	Usage: python cleantax2rcc.py <cleantax input file>

2. Running the RCC reasoner
Run the RCC reasoner, where the <inputfile> is in uber-mir format. If <optimizaiton_flag> is set to be "true", then the input file will apply all congruence relation before run the reasoner, if set to be "false", then the reasoner will run without this optimization.
	Usage: python runrcc <inputfile> <optimization_flag>

3. Visualize the R32 composition table
Visualize the R32 composition table, show the compositional rules of suggested node (in number 0-31), or put "all" to show all nodes.
	Usage: python r32tableViz.py <output_file> <node (number)>

4. Show the deduced graph of a pair of concept
During the process of RCC reasoning, show how do a pair of concept deduced, it will create graph file "pic.dot".
	Usage: python showdeduced.py <input_file> <optimization_flag> <concept1> <concept2>
	       python viz.py

