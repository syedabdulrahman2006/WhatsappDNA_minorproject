# GroupDNA — Hostel Bois 4ever

GroupDNA is a Python-based WhatsApp group analytics project that turns a raw WhatsApp export into a readable behavioural report. The project analyzes the supplied synthetic `hostel_bois.txt` dataset for the fictional group “Hostel Bois 4ever”. It parses timestamped messages, handles WhatsApp system messages, media placeholders, deleted messages, empty lines, and continuation lines, and then produces activity, vocabulary, response, and personality insights.

The submission is intentionally built under the project constraints. It uses Python fundamentals, file I/O, dictionaries, lists, sets, tuples, loops, conditionals, functions, string methods, `datetime`, and NumPy. It does **not** use pandas, matplotlib, seaborn, plotly, regex, `collections.Counter`, `collections.defaultdict`, NLTK, scikit-learn, AI/ML libraries, or a pre-built WhatsApp analyzer.

The notebook contains all eight mandatory features: a robust chat parser, group overview, busiest day/hour analysis, a 6×24 NumPy activity heatmap, top-word frequency analysis, response speed and silent streaks, quantitative personality archetype detection, and a final formatted report. The six supplied participants are assigned the expected archetypes: Rahul as The Spammer, Priya as The Group Mom, Aman as The Night Owl, Karan as The Storyteller, Neha as The Drama Queen, and Vikas as The Ghost. A ninth bonus archetype, The Chai Commander, is also included as an additional signal.

## Dataset validation

The parser successfully identifies **3,174 messages**, **6 participants**, **4 system messages**, **32 media entries**, and **15 deleted messages** from the supplied export. The NumPy heatmap row totals match the per-person message counts.

## How to run

1. Open `GroupDNA_Hostel_Bois.ipynb` in Google Colab or Jupyter.
2. Upload `hostel_bois.txt` into the notebook's working directory.
3. Run the cells from top to bottom.
4. The final cell prints the complete GroupDNA report.

The executed notebook is included with outputs already generated so the final report can be reviewed immediately.

## Screenshot

See `groupdna_report.png` for the final formatted report output.

## Project constraints

**Allowed:** Python fundamentals, NumPy, `open()`, `datetime`, lists, dictionaries, sets, tuples, loops, functions, string methods, comprehensions, sorting, and f-strings.

**Forbidden:** pandas, plotting libraries, regex, `collections` counters/defaultdicts, external chat datasets, pre-built analyzers, and AI/ML libraries.
