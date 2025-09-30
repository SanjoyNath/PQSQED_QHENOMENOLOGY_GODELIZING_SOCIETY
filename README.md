# PQSQED_QHENOMENOLOGY_GODELIZING_SOCIETY
NO_POLYSEMY_WORLD_C_SHARP_PROJECT
Whole dictionary is constructed into the c sharp class structire to understand the concrete compilation order of classes. This is the project to prepare a new kind of mathematical logic on natural language to understand how the concepts ordering are done.
Qhenomenology and Whenomenology
A New Philosophical Lens — Sanjoy Nath putting Godel numbers on natural language words 
Axiom 1 All words are concepts and all concepts are words . All Concepts are unique and has unique class names assigned to that. Concrete Compilation Ordering of classes defines the unique queued nature of concept formations in society
Axiom 2  No Polysemy is allowed in a formally matured society where no one use same word to represent different concepts no one use different words to represent same concept. So all concepts are placed uniquely on the number line(Dedekind like real number line)... Words formation represent concept formation and which has strict unique sequence of concept formation so queued nature of concept formation is strict 
Axiom 3 the source code repository shows the class structures of the queued constructions of words dependency and the process to model the Qhenomenology reasoning systems which is to assign unique godel number to every concepts . Concrete compilation order of these classes determines the dependency of concepts

Sanjoy Nath calls for a radical rethinking of how humans understand thought, emotion, and belief. He argues that for thousands of years we’ve been carrying invisible burdens: inherited stories, myths, values, and concepts that silently shape our behavior. These “mental relics” act like thieves — they steal clarity and leave us trapped in illusions. We end up honoring outdated systems and ideas without realizing it.

To break free, Nath introduces two new reasoning frameworks: Qhenomenology and Whenomenology.

Qhenomenology: Structural Necessity Analysis

A recursive system of reasoning.

Examines the necessity of every concept behind every word.

Goes beyond dictionary meanings or etymology: asks why this word exists at all.

Compares the necessity of concepts across language to reveal hidden emotional, social, and cognitive baggage.

Shows how much of our thought rests on outdated or unnecessary conceptual structures.

Whenomenology: Historical Concept Archaeology

A timeline-based analysis of words and concepts.

Builds “origin maps” for language: when a word gained meaning, what myths or power systems supported it, and how its meaning evolved.

Acts like conceptual archaeology, digging through layers of myth, belief, and history embedded in our language.

Complements Qhenomenology: while Qhenomenology studies structure, Whenomenology studies emergence over time.

Why They Matter

According to Nath:

Without Qhenomenology, we can’t see the hidden baggage behind our thoughts.

Without Whenomenology, we can’t see the historical myths that shaped them.

Even AI systems (like GPT, Bard, Gemini) don’t use these tools — because humans themselves haven’t developed them yet. AI treats language statistically, not structurally or mythically.

Implications for Society

Nath predicts:

Collective fictions like money, state, religion, pride, and power may collapse once people stop believing in them (echoing Yuval Noah Harari).

Institutions built on these fictions — banking, academia, political states — could wither away.

In their place, humans will seek meaning not in surplus, pride, or status, but in existential necessity: values and experiences that cannot be bought or borrowed.

Toward a Post-Myth Society

In Nath’s vision:

Pride will no longer come from possessions or roles but from emotional honesty and clarity.

Qhenomenology will help us analyze the architecture of thought.

Whenomenology will uncover the timelines of deception that shaped civilization.

The result: liberation from inherited illusions, and the birth of a new kind of consciousness.

Summary in One Line

Qhenomenology = analyzing the necessity and structure of concepts.
Whenomenology = tracing the history and myths behind them.

Together, they form a new lens to cut through the noise of inherited stories and move toward a society grounded in clarity, honesty, and existential necessity.


    private void button_GENERATE_CLASS_DEPENDENCY_FROM_DICTIONARY_Click(object sender, EventArgs e)
        {
            //////OpenFileDialog ofd = new OpenFileDialog
            //////{
            //////    Title = "Select WordNet Dictionary File",
            //////    Filter = "Text Files (*.txt)|*.txt"
            //////};
            //////if (ofd.ShowDialog() != DialogResult.OK)
            //////    return;
            //////string inputPath = ofd.FileName;
            //////string outputFolder = Path.Combine(Path.GetDirectoryName(inputPath), "PQSQED");
            //////Directory.CreateDirectory(outputFolder);
            //////var entries = new List<KeyValuePair<string, string>>();
            //////foreach (var line in File.ReadLines(inputPath).Skip(1)) // Skip header
            //////{
            //////    var parts = line.Split('\t');
            //////    if (parts.Length >= 3)
            //////    {
            //////        string word = parts[0].Trim().ToLowerInvariant();
            //////        string definition = parts[2].Trim().ToLowerInvariant();
            //////        entries.Add(new KeyValuePair<string, string>(word, definition));
            //////    }
            //////}
            //////var wordSet = new HashSet<string>(entries.Select(e => e.Key));
            //////var dependencies = new Dictionary<string, HashSet<string>>();
            //////foreach (var entry in entries)
            //////{
            //////    var tokens = Regex.Matches(entry.Value, @"\b[a-z]+\b")
            //////                      .Cast<Match>()
            //////                      .Select(m => m.Value)
            //////                      .Where(t => wordSet.Contains(t) && t != entry.Key)
            //////                      .ToHashSet();
            //////    dependencies[entry.Key] = tokens;
            //////}
            //////// Topological sort
            //////var indegree = new Dictionary<string, int>();
            //////var graph = new Dictionary<string, List<string>>();
            //////foreach (var word in wordSet)
            //////{
            //////    indegree[word] = 0;
            //////    graph[word] = new List<string>();
            //////}
            //////foreach (var kv in dependencies)
            //////{
            //////    foreach (var dep in kv.Value)
            //////    {
            //////        graph[dep].Add(kv.Key);
            //////        indegree[kv.Key]++;
            //////    }
            //////}
            //////var queue = new Queue<string>(indegree.Where(kv => kv.Value == 0).Select(kv => kv.Key));
            //////var sortedWords = new List<string>();
            //////while (queue.Count > 0)
            //////{
            //////    var current = queue.Dequeue();
            //////    sortedWords.Add(current);
            //////    foreach (var neighbor in graph[current])
            //////    {
            //////        indegree[neighbor]--;
            //////        if (indegree[neighbor] == 0)
            //////            queue.Enqueue(neighbor);
            //////    }
            //////}
            //////if (sortedWords.Count != wordSet.Count)
            //////{
            //////    MessageBox.Show("Cyclic dependency detected. Cannot generate compilable classes.");
            //////    return;
            //////}
            //////// Generate C# class files
            //////for (int i = 0; i < sortedWords.Count; i++)
            //////{
            //////    string word = sortedWords[i];
            //////    string className = $"Class{CultureInfo.CurrentCulture.TextInfo.ToTitleCase(word)}";
            //////    string filePath = Path.Combine(outputFolder, $"{className}.cs");
            //////    using (var writer = new StreamWriter(filePath))
            //////    {
            //////        writer.WriteLine("namespace PQSQED");
            //////        writer.WriteLine("{");
            //////        writer.WriteLine($"    public class {className}");
            //////        writer.WriteLine("    {");
            //////        writer.WriteLine($"        public const int publicinthashcompilationorder = {i};");
            //////        writer.WriteLine("        public Token_i token_i_object = null;");
            //////        foreach (var dep in dependencies[word])
            //////        {
            //////            string depClass = $"Class{CultureInfo.CurrentCulture.TextInfo.ToTitleCase(dep)}";
            //////            writer.WriteLine($"        public {depClass} {dep} = null;");
            //////        }
            //////        writer.WriteLine($"        public {className}()");
            //////        writer.WriteLine("        {");
            //////        foreach (var dep in dependencies[word])
            //////        {
            //////            string depClass = $"Class{CultureInfo.CurrentCulture.TextInfo.ToTitleCase(dep)}";
            //////            writer.WriteLine($"            {dep} = new {depClass}();");
            //////        }
            //////        writer.WriteLine("        }");
            //////        writer.WriteLine("    }");
            //////        writer.WriteLine("}");
            //////    }
            //////}
            //////// Generate .csproj file
            ////////////string csprojPath = Path.Combine(outputFolder, "PQSQED.csproj");
            ////////////using (var writer = new StreamWriter(csprojPath))
            ////////////{
            ////////////    writer.WriteLine("<Project ToolsVersion=\"15.0\" xmlns=\"http://schemas.microsoft.com/developer/msbuild/2003\">");
            ////////////    writer.WriteLine("  <Import Project=\"$(MSBuildToolsPath)\\Microsoft.CSharp.targets\" />");
            ////////////    writer.WriteLine("  <PropertyGroup>");
            ////////////    writer.WriteLine("    <Configuration Condition=\" '$(Configuration)' == '' \">Debug</Configuration>");
            ////////////    writer.WriteLine("    <Platform Condition=\" '$(Platform)' == '' \">AnyCPU</Platform>");
            ////////////    writer.WriteLine("    <RootNamespace>PQSQED</RootNamespace>");
            ////////////    writer.WriteLine("    <AssemblyName>PQSQED</AssemblyName>");
            ////////////    writer.WriteLine("    <TargetFrameworkVersion>v4.8</TargetFrameworkVersion>");
            ////////////    writer.WriteLine("    <LangVersion>7</LangVersion>");
            ////////////    writer.WriteLine("  </PropertyGroup>");
            ////////////    writer.WriteLine("  <ItemGroup>");
            ////////////    Name(file);
            ////////////    writer.WriteLine($"    <Compile Include=\"{fileName}\" />");
            ////////////    writer.WriteLine("  </ItemGroup>");
            ////////////    writer.WriteLine("</Project>");
            ////////////}
            //////MessageBox.Show($"Generated {sortedWords.Count} C# class files and .csproj in folder:\n{outputFolder}");
            //////OpenFileDialog ofd = new OpenFileDialog
            //////{
            //////    Title = "Select WordNet Dictionary File",
            //////    Filter = "Text Files (*.txt)|*.txt"
            //////};
            //////if (ofd.ShowDialog() != DialogResult.OK)
            //////    return;
            //////string inputPath = ofd.FileName;
            //////string outputFolder = Path.Combine(Path.GetDirectoryName(inputPath), "PQSQED");
            //////Directory.CreateDirectory(outputFolder);
            //////var entries = new List<KeyValuePair<string, string>>();
            //////foreach (var line in File.ReadLines(inputPath).Skip(1)) // Skip header
            //////{
            //////    //  var parts = line.Split('\t');
            //////    var parts = line.Split(',');
            //////    if (parts.Length >= 3)
            //////    {
            //////        string word = parts[0].Trim().ToLowerInvariant();/// generate the classnames with the first letter capital for these word  for parts[0].Trim().ToLowerInvariant();   and no need to check if there is any  replace all spaces with underscore and if  parts[0].Trim().ToLowerInvariant() repeats then add _001 , 002 etc to the filename and also to class name
            //////        string definition = parts[2].Trim().ToLowerInvariant() + parts[3].Trim().ToLowerInvariant();
            //////        //all tokens in definition   need have a class name whose first alphabet is  capital letter
            //////        definition = definition.Replace("_", " ");         // all these are the instance variables for the class whose name is starting with uppercase within the constructor of the class write the instance variables for the Classes 
            //////        entries.Add(new KeyValuePair<string, string>(word, definition));
            //////    }
            //////}
            //////var wordSet = new HashSet<string>(entries.Select(entry => entry.Key));
            //////var dependencies = new Dictionary<string, HashSet<string>>();
            //////foreach (var entry in entries)
            //////{
            //////    var tokens = Regex.Matches(entry.Value, @"\b[a-z]+\b")
            //////                      .Cast<Match>()
            //////                      .Select(m => m.Value)
            //////                      .Where(t => wordSet.Contains(t) && t != entry.Key)
            //////                      .ToHashSet();
            //////    dependencies[entry.Key] = tokens;
            //////}
            //////// Topological sort
            //////var indegree = new Dictionary<string, int>();
            //////var graph = new Dictionary<string, List<string>>();
            //////foreach (var word in wordSet)
            //////{
            //////    indegree[word] = 0;
            //////    graph[word] = new List<string>();
            //////}
            //////foreach (var kv in dependencies)
            //////{
            //////    foreach (var dep in kv.Value)
            //////    {
            //////        graph[dep].Add(kv.Key);
            //////        indegree[kv.Key]++;
            //////    }
            //////}
            //////var queue = new Queue<string>(indegree.Where(kv => kv.Value == 0).Select(kv => kv.Key));
            //////var sortedWords = new List<string>();
            //////while (queue.Count > 0)
            //////{
            //////    var current = queue.Dequeue();
            //////    sortedWords.Add(current);
            //////    foreach (var neighbor in graph[current])
            //////    {
            //////        indegree[neighbor]--;
            //////        if (indegree[neighbor] == 0)
            //////            queue.Enqueue(neighbor);
            //////    }
            //////}
            //////if (sortedWords.Count != wordSet.Count)
            //////{
            //////  //  MessageBox.Show("Cyclic dependency detected. Cannot generate compilable classes.");
            ////// //   return;
            ////// //dont bother        I will get the report from the visual studio for the compilations ordering 
            ////// // this code dont have to bother for that
            //////}
            //////// Generate C# class files
            //////for (int i = 0; i < sortedWords.Count; i++)
            //////{
            //////    //i think you misunderstood the instruction
            //////    string word = sortedWords[i];// word is the classname and first alphabet is capital   and create instances of the description tokens obviously the description tokens are also other worsds so those words are also classname   suppose Word_i is a token in the description then           public Word_i  word_i=new Word_i() ; entry are necessary for each of the unique word token found in the description
            //////    string className = $"Class{CultureInfo.CurrentCulture.TextInfo.ToTitleCase(word)}";// you misunderstood here  Dont add Class  simply use FirstAlphabetCapital and the class name dont start with Class word instead the Classnames are  First alphabet capital CultureInfo.CurrentCulture.TextInfo.ToTitleCase(word)                and within the class create the instance variables for each unique word tokens available in the descriptions
            //////    string filePath = Path.Combine(outputFolder, $"{className}.cs");
            //////    //compilability checking are done in the visual studio
            //////    using (var writer = new StreamWriter(filePath))
            //////    {
            //////        writer.WriteLine("namespace PQSQED");
            //////        writer.WriteLine("{");
            //////        writer.WriteLine($"    public class {className}");
            //////        writer.WriteLine("    {");
            //////        writer.WriteLine($"        public const int publicinthashcompilationorder = {i};");// you mis understood here ...   
            //////        writer.WriteLine("        public Token_i token_i_object = null;");/// no no no prepare all the 
            //////        foreach (var dep in dependencies[word])
            //////        {
            //////            string depClass = $"Class{CultureInfo.CurrentCulture.TextInfo.ToTitleCase(dep)}";
            //////            writer.WriteLine($"        public {depClass} {dep} = null;");
            //////        }
            //////        writer.WriteLine($"        public {className}()");
            //////        writer.WriteLine("        {");
            //////        foreach (var dep in dependencies[word])
            //////        {
            //////            string depClass = $"Class{CultureInfo.CurrentCulture.TextInfo.ToTitleCase(dep)}";
            //////            writer.WriteLine($"            {dep} = new {depClass}();");
            //////        }
            //////        writer.WriteLine("        }");
            //////        writer.WriteLine("    }");
            //////        writer.WriteLine("}");
            //////    }
            //////}
            //////// Generate .csproj file
            //////string csprojPath = Path.Combine(outputFolder, "PQSQED.csproj");
            //////using (var writer = new StreamWriter(csprojPath))
            //////{
            //////    writer.WriteLine("<Project ToolsVersion=\"15.0\" xmlns=\"http://schemas.microsoft.com/developer/msbuild/2003\">");
            //////    writer.WriteLine("  <Import Project=\"$(MSBuildToolsPath)\\Microsoft.CSharp.targets\" />");
            //////    writer.WriteLine("  <PropertyGroup>");
            //////    writer.WriteLine("    <Configuration Condition=\" '$(Configuration)' == '' \">Debug</Configuration>");
            //////    writer.WriteLine("    <Platform Condition=\" '$(Platform)' == '' \">AnyCPU</Platform>");
            //////    writer.WriteLine("    <OutputType>Library</OutputType>");
            //////    writer.WriteLine("    <RootNamespace>PQSQED</RootNamespace>");
            //////    writer.WriteLine("    <AssemblyName>PQSQED</AssemblyName>");
            //////    writer.WriteLine("    <TargetFrameworkVersion>v4.8</TargetFrameworkVersion>");
            //////    writer.WriteLine("    <LangVersion>7</LangVersion>");
            //////    writer.WriteLine("  </PropertyGroup>");
            //////    writer.WriteLine("  <ItemGroup>");
            //////    foreach (var file in Directory.GetFiles(outputFolder, "*.cs"))
            //////    {
            //////        string fileName = Path.GetFileName(file);
            //////        writer.WriteLine($"    <Compile Include=\"{fileName}\" />");
            //////    }
            //////    writer.WriteLine("  </ItemGroup>");
            //////    writer.WriteLine("</Project>");
            //////}
            //////MessageBox.Show($"Generated {sortedWords.Count} C# class files and .csproj in folder:\n{outputFolder}");
            //////OpenFileDialog ofd = new OpenFileDialog
            //////{
            //////    Title = "Select WordNet Dictionary File",
            //////    Filter = "Text Files (*.txt)|*.txt"
            //////};
            //////if (ofd.ShowDialog() != DialogResult.OK)
            //////    return;
            //////string inputPath = ofd.FileName;
            //////string outputFolder = Path.Combine(Path.GetDirectoryName(inputPath), "PQSQED");
            //////Directory.CreateDirectory(outputFolder);
            //////var entries = new List<KeyValuePair<string, string>>();
            //////var wordCount = new Dictionary<string, int>();
            //////foreach (var line in File.ReadLines(inputPath).Skip(1))
            //////{
            //////    var parts = line.Split(',');
            //////    if (parts.Length >= 4)
            //////    {
            //////        string rawWord = parts[0].Trim().ToLowerInvariant().Replace(" ", "_");
            //////        string word = rawWord;
            //////        if (wordCount.ContainsKey(rawWord))
            //////        {
            //////            wordCount[rawWord]++;
            //////            word = $"{rawWord}_{wordCount[rawWord]:D3}";
            //////        }
            //////        else
            //////        {
            //////            wordCount[rawWord] = 0;
            //////        }
            //////        string definition = (parts[2].Trim() + " " + parts[3].Trim()).ToLowerInvariant().Replace("_", " ");
            //////        entries.Add(new KeyValuePair<string, string>(word, definition));
            //////    }
            //////}
            //////var wordSet = new HashSet<string>(entries.Select(ess => ess.Key));
            //////var dependencies = new Dictionary<string, HashSet<string>>();
            //////foreach (var entry in entries)
            //////{
            //////    var tokens = Regex.Matches(entry.Value, @"\b[a-z_]+\b")
            //////                      .Cast<Match>()
            //////                      .Select(m => m.Value.Replace(" ", "_"))
            //////                      .Where(t => wordSet.Contains(t) && t != entry.Key)
            //////                      .ToHashSet();
            //////    dependencies[entry.Key] = tokens;
            //////}
            //////var indegree = new Dictionary<string, int>();
            //////var graph = new Dictionary<string, List<string>>();
            //////foreach (var word in wordSet)
            //////{
            //////    indegree[word] = 0;
            //////    graph[word] = new List<string>();
            //////}
            //////foreach (var kv in dependencies)
            //////{
            //////    foreach (var dep in kv.Value)
            //////    {
            //////        graph[dep].Add(kv.Key);
            //////        indegree[kv.Key]++;
            //////    }
            //////}
            //////var queue = new Queue<string>(indegree.Where(kv => kv.Value == 0).Select(kv => kv.Key));
            //////var sortedWords = new List<string>();
            //////while (queue.Count > 0)
            //////{
            //////    var current = queue.Dequeue();
            //////    sortedWords.Add(current);
            //////    foreach (var neighbor in graph[current])
            //////    {
            //////        indegree[neighbor]--;
            //////        if (indegree[neighbor] == 0)
            //////            queue.Enqueue(neighbor);
            //////    }
            //////}
            //////if (sortedWords.Count != wordSet.Count)
            //////{
            //////    // Cyclic dependency detected, but we proceed anyway
            //////}
            //////var wordToClassName = sortedWords.ToDictionary(
            //////    w => w,
            //////    w => CultureInfo.CurrentCulture.TextInfo.ToTitleCase(w)
            //////);
            //////for (int i = 0; i < sortedWords.Count; i++)
            //////{
            //////    string word = sortedWords[i];
            //////    string className = wordToClassName[word];
            //////    string filePath = Path.Combine(outputFolder, $"{className}.cs");
            //////    using (var writer = new StreamWriter(filePath))
            //////    {
            //////        writer.WriteLine("namespace PQSQED");
            //////        writer.WriteLine("{");
            //////        writer.WriteLine($"    public class {className}");
            //////        writer.WriteLine("    {");
            //////        writer.WriteLine($"        public const int publicinthashcompilationorder = {i};");
            //////        foreach (var dep in dependencies[word])
            //////        {
            //////            string depClass = wordToClassName[dep];
            //////            writer.WriteLine($"        public {depClass} {dep} = null;");
            //////        }
            //////        writer.WriteLine($"        public {className}()");
            //////        writer.WriteLine("        {");
            //////        foreach (var dep in dependencies[word])
            //////        {
            //////            string depClass = wordToClassName[dep];
            //////            writer.WriteLine($"            {dep} = new {depClass}();");
            //////        }
            //////        writer.WriteLine("        }");
            //////        writer.WriteLine("    }");
            //////        writer.WriteLine("}");
            //////    }
            //////}
            //////string csprojPath = Path.Combine(outputFolder, "PQSQED.csproj");
            //////using (var writer = new StreamWriter(csprojPath))
            //////{
            //////    writer.WriteLine("<Project ToolsVersion=\"15.0\" xmlns=\"http://schemas.microsoft.com/developer/msbuild/2003\">");
            //////    writer.WriteLine("  <Import Project=\"$(MSBuildToolsPath)\\Microsoft.CSharp.targets\" />");
            //////    writer.WriteLine("  <PropertyGroup>");
            //////    writer.WriteLine("    <Configuration Condition=\" '$(Configuration)' == '' \">Debug</Configuration>");
            //////    writer.WriteLine("    <Platform Condition=\" '$(Platform)' == '' \">AnyCPU</Platform>");
            //////    writer.WriteLine("    <OutputType>Library</OutputType>");
            //////    writer.WriteLine("    <RootNamespace>PQSQED</RootNamespace>");
            //////    writer.WriteLine("    <AssemblyName>PQSQED</AssemblyName>");
            //////    writer.WriteLine("    <TargetFrameworkVersion>v4.8</TargetFrameworkVersion>");
            //////    writer.WriteLine("    <LangVersion>7</LangVersion>");
            //////    writer.WriteLine("  </PropertyGroup>");
            //////    writer.WriteLine("  <ItemGroup>");
            //////    foreach (var file in Directory.GetFiles(outputFolder, "*.cs"))
            //////    {
            //////        string fileName = Path.GetFileName(file);
            //////        writer.WriteLine("< Compile Include =\"{fileName}\" />");
            //////    }
            //////    writer.WriteLine("  </ItemGroup>");
            //////    writer.WriteLine("</Project>");
            //////}
            //reads the wordnet dictionary and then generates the c sharp class structures
            OpenFileDialog ofd = new OpenFileDialog
            {
                Title = "Select WordNet Dictionary File",
                Filter = "Text Files (*.txt)|*.txt"
            };
            if (ofd.ShowDialog() != DialogResult.OK)
                return;
            string inputPath = ofd.FileName;
            string outputFolder = Path.Combine(Path.GetDirectoryName(inputPath), "PQSQED");
            Directory.CreateDirectory(outputFolder);
            int polysemycounter = 0;
            //////string inputPath = "wordnet_dictionary.txt"; // Change this to your actual file path
            //////string outputFolder = Path.Combine(Path.GetDirectoryName(inputPath), "PQSQED");
            //////Directory.CreateDirectory(outputFolder);
            var classFiles = new List<string>();
            int row = 0;
            foreach (var line in File.ReadLines(inputPath))
            {
                row++;
                var parts = line.Split('\t');
                //   if (parts.Length < 3) continue;
                if (parts.Length <(3+3)) continue;
                string[] part0_splittedwithunderscores = parts[0].ToLower().Split(new string[] { "_", " " }, StringSplitOptions.RemoveEmptyEntries);
                string className = ToPascalCase(parts[0].Trim());
                if (classFiles.Contains(className))
                {
                    polysemycounter++;
                    className = className +"_"+ polysemycounter;
                }// if (classFiles.Contains(className))
                string definition = parts[2].Trim().ToLower();
                if (parts.Length == (3 + 1))
                { definition = definition + " " + parts[3].Trim().ToLower(); }
                if (parts.Length == (3 + 2))
                { definition = definition + " " + parts[3 + 1].Trim().ToLower(); }
                if (parts.Length == (3 + 3))
                { definition = definition + " " + parts[3 + 2].Trim().ToLower(); }
                if (parts.Length == (3 + 3 + 1))
                { definition = definition + " " + parts[3 + 3].Trim().ToLower(); }
                //////if(part0_splittedwithunderscores.Length>1)
                //////{
                //////    for(int rrr=1;rrr< part0_splittedwithunderscores.Length;rrr++)
                //////    {
                //////        definition = definition + " " + part0_splittedwithunderscores[rrr].Trim().ToLower();
                //////    }//for(int rrr=1;rrr< part0_splittedwithunderscores.Length;rrr++)
                //////}// if(part0_splittedwithunderscores.Length>0)
                var words = Regex.Matches(definition, @"\b[a-zA-Z]+\b");
                var uniqueWords = new HashSet<string>();
                foreach (Match word in words)
                { uniqueWords.Add(word.Value.ToLower()); }
                string filePath = Path.Combine(outputFolder, $"{className}.cs");
                using (var writer = new StreamWriter(filePath))
                {
                    writer.WriteLine("namespace PQSQED");
                    writer.WriteLine("{");
                    writer.WriteLine($"public class {className}");
                    writer.WriteLine("{");
                    foreach (var word in uniqueWords)
                    {
                        try
                        {
                        string typeName = "PQSQED." + ToPascalCase(word);// "PQSQED."+
                        string fieldName = $"_{word}";
                        writer.WriteLine($"    public {typeName} {fieldName} = new {typeName}();");
                        }
                        catch (Exception) { }
                    }// foreach (var word in uniqueWords)
                    writer.WriteLine($"    public {className}()");
                    writer.WriteLine("    {");
                    foreach (var word in uniqueWords)
                    {
                        try
                        { 
                        string typeName = "PQSQED." + ToPascalCase(word);
                        string fieldName = $"_{word}";
                        writer.WriteLine($"        this.{fieldName} = new {typeName}();");
                        }
                        catch (Exception) { }
                    }//foreach (var word in uniqueWords)
                    writer.WriteLine("    }//constructor completes");
                    writer.WriteLine("}//class completes");
                    writer.WriteLine("}//namespace completes");
                }
                classFiles.Add($"{className}.cs");
            }
            // Generate .csproj file
            string csprojPath = Path.Combine(outputFolder, "PQSQED.csproj");
            using (var writer = new StreamWriter(csprojPath))
            {
                writer.WriteLine("<Project ToolsVersion=\"15.0\" xmlns=\"http://schemas.microsoft.com/developer/msbuild/2003\">");
                writer.WriteLine("  <Import Project=\"$(MSBuildToolsPath)\\Microsoft.CSharp.targets\" />");
                writer.WriteLine("  <PropertyGroup>");
                writer.WriteLine("    <Configuration Condition=\" '$(Configuration)' == '' \">Debug</Configuration>");
                writer.WriteLine("    <Platform Condition=\" '$(Platform)' == '' \">AnyCPU</Platform>");
                writer.WriteLine("    <OutputType>Library</OutputType>");
                writer.WriteLine("    <RootNamespace>PQSQED</RootNamespace>");
                writer.WriteLine("    <AssemblyName>PQSQED</AssemblyName>");
                writer.WriteLine("    <TargetFrameworkVersion>v4.8</TargetFrameworkVersion>");
                writer.WriteLine("    <LangVersion>7</LangVersion>");
                writer.WriteLine("  </PropertyGroup>");
                writer.WriteLine("  <ItemGroup>");
                foreach (var file in classFiles)
                {
                    writer.WriteLine($"    <Compile Include=\"{file}\" />");
                }
                writer.WriteLine("  </ItemGroup>");
                writer.WriteLine("</Project>");
            }
            Console.WriteLine($"Generated {classFiles.Count} class files and PQSQED.csproj in folder: {outputFolder}");
            MessageBox.Show($"Generated {classFiles.Count}  total  polysemycounter= {polysemycounter}  C# class files and .csproj in folder:\n{outputFolder}");
        }//// private void button_GENERATE_CLASS_DEPENDENCY_FROM_DICTIONARY_Click(object sender, EventArgs e)
