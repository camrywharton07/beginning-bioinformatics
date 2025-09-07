 # AI Use Log
- Tool/model & version: Chat GPT 5
- What I asked for: Given a DNA string s with a maximum length of 1000 nucleotides, return four integers (separated by spaces) that count the occurrences of the symbols 'A', 'C', 'G', and 'T' in s.
- Snippet of prompt(s): Example Code: # Read DNA string (for example)
s = "ATGCTTCAGAAAGGTCTTACG"

# Count each nucleotide
a_count = s.count("A")
c_count = s.count("C")
g_count = s.count("G")
t_count = s.count("T")

# Print results as required
print(a_count, c_count, g_count, t_count)
Actual Code Used in Assignment:
def count_dna_bases(s):
    return {
        'A': s.count('A'),
        'C': s.count('C'),
        'G': s.count('G'),
        'T': s.count('T')
    }

# Paste your DNA string below
dna = """CCCCGTACTATAATTAGCCCCTGTCGCGTTGCAAACAAAAACGTGCCGGGCCGTTATTGGAAAGGTTTACGACCATCCATCCCGAAAGCCTTGGTGAGTTACTACTCAAAGGCTCCGCATTCTTACAGCCATTCACTGTCCGAGATACCGGGCGTCGACGTGTGTACCCGGGCTTCAATCTGCCCGGTAGCCGATAGGGTGTAGTGTGATCTTTAGACATGCTCCCCATTGTTTTACCGAGCGGGCGTCCACAGCGATAAAGTGTGCTACTACGTAAATGTACCGGTATCTTTTCTGGAGCCCGCCCAGTACGGCAGTGTAAAACCGAATGCGAGCTAGAGACCCCCGTCATACCAGCCTAGTCTAACAAATCAAGGCCCATGGGTCGTATGTTGATCGAGTCCGGGATCGTTGGATTAATATCAAAATTGTGGAGGTGAACCCATGTAAGAAAGAGCTCTGGTCATTGCAGATTGACTCCAGTAGCTGTTTACTTGCTTCCTCAACAACACATTCCAACCGTCTAGCAACGAGTGCCGCGGGAAACGGGTACTAGGTGATTTTTGGGAGACAGAAGCGCCGGCCTAACTGCTCAGGGTATGAACCCTAATTTTAAGGTCTAGTCTCAAATGATTGCTATGCCGTTCTAGGCAGCCTATTCGCAAAGAAGCGCGAAGCCTGAGGCCCGAACCCCGAAATACGCGTTGACGAAACTATTTACTATTTTGCTGAGCCTATCACCAATAAAAGAGAATCCAGGCAGATGGTGATGCTACCCTGCGTGTCGCTCCCCAGGACTGCTTAGTTGCGAAAAGAAGTTGATTGGCCA"""

# Count and display
counts = count_dna_bases(dna)

# Print output in one line (like Rosalind expects)
print(counts['A'], counts['C'], counts['G'], counts['T'])

- What I changed before committing: Before finalizing, I modified my code to print the output in a single line, as expected by Rosalind. This change was made to ensure the correctness of the provided code.
- How I verified correctness (tests, sample data): I verified the accuracy of my work through trial and error. I requested an example code from ChatGPT for counting DNA nucleotides and used that practice code in Google Colab. This helped me ensure everything was correct before downloading the dataset for submission.
