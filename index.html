import { useState, useEffect, useRef } from "react";

const STYLES = `
@import url('https://fonts.googleapis.com/css2?family=Lexend:wght@300;400;500;600;700&family=Fira+Code:wght@400;500&family=Bebas+Neue&display=swap');
*{box-sizing:border-box;margin:0;padding:0}
:root{--bg:#06091A;--bg2:#0C1230;--bg3:#121A38;--bg4:#1A2448;--acc:#7C3AED;--acc2:#06B6D4;--acc3:#10B981;--warn:#F59E0B;--danger:#EF4444;--text:#E8EDF5;--text2:#8B99B5;--border:#1E2D52;--cbg:#040710}
.lt{--bg:#F0F4FF;--bg2:#E3EAFF;--bg3:#D4E0FF;--bg4:#C5D3FF;--acc:#7C3AED;--acc2:#0284C7;--acc3:#059669;--warn:#D97706;--danger:#DC2626;--text:#0F172A;--text2:#475569;--border:#BFCBF5;--cbg:#1E1B4B}
body,html{font-family:'Lexend',sans-serif;background:var(--bg);color:var(--text);height:100%}
@keyframes fadeUp{from{opacity:0;transform:translateY(16px)}to{opacity:1;transform:translateY(0)}}
@keyframes slideL{from{opacity:0;transform:translateX(-16px)}to{opacity:1;transform:translateX(0)}}
@keyframes charBounce{0%,100%{transform:translateY(0) scale(1)}50%{transform:translateY(-10px) scale(1.1)}}
@keyframes windowSlide{0%{left:0}50%{left:60px}100%{left:120px}}
@keyframes kmpMatch{0%{background:var(--bg4)}100%{background:var(--acc3)}}
@keyframes pulse{0%,100%{opacity:1}50%{opacity:.4}}
@keyframes spin{to{transform:rotate(360deg)}}
@keyframes glow{0%,100%{box-shadow:0 0 8px rgba(124,58,237,.4)}50%{box-shadow:0 0 24px rgba(124,58,237,.8)}}
.fade{animation:fadeUp .45s ease}
.slide{animation:slideL .4s ease}
pre,code,.mono{font-family:'Fira Code',monospace}
.hd{font-family:'Bebas Neue',sans-serif;letter-spacing:.05em}
.sb::-webkit-scrollbar{width:4px}.sb::-webkit-scrollbar-track{background:transparent}.sb::-webkit-scrollbar-thumb{background:var(--border);border-radius:2px}
.btn{cursor:pointer;border:none;font-family:'Lexend',sans-serif;transition:all .2s}
.chip{display:inline-flex;align-items:center;padding:2px 10px;border-radius:999px;font-size:12px;font-weight:500}
.tag-e{background:rgba(16,185,129,.15);color:#34D399}.tag-m{background:rgba(245,158,11,.15);color:#FCD34D}.tag-h{background:rgba(239,68,68,.15);color:#FCA5A5}.tag-f{background:rgba(124,58,237,.2);color:#A78BFA}
`;

// ═══════════════════════════════════ CONTENT DATA ═══════════════════════════════════

const NAV = [
  {id:0,icon:"🏠",label:"Welcome"},
  {id:1,icon:"🔤",label:"What is a String?"},
  {id:2,icon:"🔢",label:"ASCII & Unicode"},
  {id:3,icon:"📍",label:"Indexing & Traversal"},
  {id:4,icon:"✂️",label:"Substrings & Subsequences"},
  {id:5,icon:"🔄",label:"Palindromes"},
  {id:6,icon:"📊",label:"Frequency & Hashing"},
  {id:7,icon:"👉👈",label:"Two Pointer"},
  {id:8,icon:"🪟",label:"Sliding Window"},
  {id:9,icon:"🔍",label:"Pattern Matching (KMP)"},
  {id:10,icon:"🧠",label:"Problem Identification"},
  {id:11,icon:"💻",label:"LeetCode Top 25"},
  {id:12,icon:"🔥",label:"Practice 50 Problems"},
  {id:13,icon:"🚀",label:"Approach Builder"},
  {id:14,icon:"📋",label:"Cheatsheet"},
];

const CODE = {
  basic_cpp:`// A string is just an array of characters!
#include <iostream>
#include <string>
using namespace std;

int main() {
    string s = "Hello";
    
    // Each character has an index
    // H  e  l  l  o
    // 0  1  2  3  4
    
    cout << s[0];        // H
    cout << s.length();  // 5
    cout << s[s.size()-1]; // o (last char)
    
    // Traverse the string
    for (int i = 0; i < s.length(); i++) {
        cout << s[i] << " ";
    }
    // Range-based loop (easier!)
    for (char c : s) {
        cout << c << " ";
    }
    return 0;
}`,
  basic_py:`# A string is just a sequence of characters!

s = "Hello"

# Each character has an index
# H  e  l  l  o
# 0  1  2  3  4

print(s[0])       # H
print(len(s))     # 5
print(s[-1])      # o (last char — Python trick!)

# Traverse the string
for i in range(len(s)):
    print(s[i], end=" ")

# Even easier in Python:
for c in s:
    print(c, end=" ")`,

  ascii_cpp:`// ASCII — every character is secretly a number!
char c = 'A';
cout << (int)c;        // 65
cout << (int)'a';      // 97
cout << (int)'0';      // 48

// Trick: lowercase = uppercase + 32
cout << (char)('A' + 32); // 'a'

// Check if lowercase
bool isLower = (c >= 'a' && c <= 'z');

// Convert to uppercase
char up = toupper('b'); // 'B'`,
  ascii_py:`# ASCII — every character is secretly a number!
c = 'A'
print(ord(c))      # 65
print(ord('a'))    # 97  
print(ord('0'))    # 48

# Trick: lowercase = uppercase + 32
print(chr(ord('A') + 32))  # 'a'

# Convert to uppercase/lowercase
print('b'.upper())  # 'B'
print('B'.lower())  # 'b'

# Check if lowercase
print('a'.islower())  # True`,

  freq_cpp:`// Count frequency of each character
#include <unordered_map>
string s = "hello";

// Method 1: Array (26 letters only)
int freq[26] = {0};
for (char c : s) {
    freq[c - 'a']++;
}
// freq[7] = 2 (h=0, e=1, l=2(twice!), o=4)

// Method 2: HashMap (any characters)
unordered_map<char,int> mp;
for (char c : s) {
    mp[c]++;
}
// mp = {'h':1, 'e':1, 'l':2, 'o':1}

// Check anagram
bool isAnagram(string a, string b) {
    if (a.length() != b.length()) return false;
    int freq[26] = {0};
    for (char c : a) freq[c-'a']++;
    for (char c : b) freq[c-'a']--;
    for (int x : freq) if (x != 0) return false;
    return true;
}`,
  freq_py:`# Count frequency of each character
from collections import Counter

s = "hello"

# Method 1: Dictionary
freq = {}
for c in s:
    freq[c] = freq.get(c, 0) + 1
# freq = {'h':1, 'e':1, 'l':2, 'o':1}

# Method 2: Counter (easiest!)
freq = Counter(s)
# Counter({'l': 2, 'h': 1, 'e': 1, 'o': 1})

# Check anagram (super clean in Python!)
def is_anagram(a, b):
    return Counter(a) == Counter(b)

print(is_anagram("listen", "silent"))  # True
print(is_anagram("hello", "world"))    # False`,

  twoptr_cpp:`// Two Pointer — Palindrome Check
// "racecar" → is it palindrome?
// r a c e c a r
// ^           ^  both 'r' ✓
//   ^ ^       move inward
//     ^ ^     'c' == 'c' ✓
//       ^     middle reached → PALINDROME!

bool isPalindrome(string s) {
    int left = 0, right = s.length() - 1;
    while (left < right) {
        if (s[left] != s[right]) return false;
        left++;    // move right
        right--;   // move left
    }
    return true;
}
// Time: O(n), Space: O(1) — Beautiful!`,
  twoptr_py:`# Two Pointer — Palindrome Check
# "racecar" → is it palindrome?
# r a c e c a r
# ^           ^  both 'r' ✓
#   ^ ^       move inward
#     ^ ^     'c' == 'c' ✓

def is_palindrome(s):
    left, right = 0, len(s) - 1
    while left < right:
        if s[left] != s[right]:
            return False
        left += 1
        right -= 1
    return True

# Python one-liner (interview trick!)
def is_palindrome_v2(s):
    return s == s[::-1]`,

  window_cpp:`// Sliding Window — Longest Substring Without Repeating
// "abcabcbb" → answer is "abc" (length 3)

int lengthOfLongestSubstring(string s) {
    unordered_map<char,int> seen;
    int left = 0, maxLen = 0;
    
    for (int right = 0; right < s.length(); right++) {
        char c = s[right];
        
        // If we've seen this char, shrink from left
        if (seen.count(c) && seen[c] >= left) {
            left = seen[c] + 1;
        }
        
        seen[c] = right;
        maxLen = max(maxLen, right - left + 1);
    }
    return maxLen;
}
// Time: O(n), Space: O(min(m,n))
// m = charset size`,
  window_py:`# Sliding Window — Longest Substring Without Repeating
# "abcabcbb" → answer is "abc" (length 3)

def length_of_longest_substring(s):
    seen = {}  # char → last index seen
    left = 0
    max_len = 0
    
    for right, c in enumerate(s):
        # If we've seen this char inside our window
        if c in seen and seen[c] >= left:
            left = seen[c] + 1  # shrink window
        
        seen[c] = right
        max_len = max(max_len, right - left + 1)
    
    return max_len

# "abcabcbb" walkthrough:
# right=0: a → window=[a], len=1
# right=1: b → window=[ab], len=2
# right=2: c → window=[abc], len=3  ← max!
# right=3: a seen! → left=1 window=[bca]`,

  kmp_cpp:`// KMP — Find pattern in text
// Text:    "ABABDABACDABABCABAB"
// Pattern: "ABABCABAB"

vector<int> computeLPS(string pat) {
    int n = pat.size();
    vector<int> lps(n, 0);
    int len = 0, i = 1;
    while (i < n) {
        if (pat[i] == pat[len]) {
            lps[i++] = ++len;
        } else {
            if (len != 0) len = lps[len-1];
            else lps[i++] = 0;
        }
    }
    return lps;
}

int kmpSearch(string text, string pattern) {
    int n = text.size(), m = pattern.size();
    vector<int> lps = computeLPS(pattern);
    int i = 0, j = 0, count = 0;
    while (i < n) {
        if (text[i] == pattern[j]) { i++; j++; }
        if (j == m) { count++; j = lps[j-1]; }
        else if (i < n && text[i] != pattern[j]) {
            if (j != 0) j = lps[j-1];
            else i++;
        }
    }
    return count; // returns number of matches
}`,
  kmp_py:`# KMP — Find pattern in text efficiently
# Key idea: never go back in text, use LPS to skip in pattern

def compute_lps(pattern):
    """LPS = Longest Proper Prefix which is also Suffix"""
    n = len(pattern)
    lps = [0] * n
    length = 0  # length of previous longest prefix suffix
    i = 1
    while i < n:
        if pattern[i] == pattern[length]:
            length += 1
            lps[i] = length
            i += 1
        else:
            if length != 0:
                length = lps[length - 1]
            else:
                lps[i] = 0
                i += 1
    return lps

def kmp_search(text, pattern):
    n, m = len(text), len(pattern)
    lps = compute_lps(pattern)
    i = j = count = 0
    while i < n:
        if text[i] == pattern[j]:
            i += 1; j += 1
        if j == m:
            count += 1
            j = lps[j-1]
        elif i < n and text[i] != pattern[j]:
            j = lps[j-1] if j != 0 else 0
            if j == 0: i += 1
    return count`,

  minwindow_cpp:`// LC 76: Minimum Window Substring
// Find smallest window in s containing all chars of t
string minWindow(string s, string t) {
    unordered_map<char,int> need, have;
    for (char c : t) need[c]++;
    
    int left = 0, formed = 0;
    int required = need.size();
    int minLen = INT_MAX, minStart = 0;
    
    for (int right = 0; right < s.size(); right++) {
        char c = s[right];
        have[c]++;
        if (need.count(c) && have[c] == need[c])
            formed++;
        
        while (formed == required) {
            // Update answer
            if (right - left + 1 < minLen) {
                minLen = right - left + 1;
                minStart = left;
            }
            // Shrink window
            char l = s[left++];
            have[l]--;
            if (need.count(l) && have[l] < need[l])
                formed--;
        }
    }
    return minLen == INT_MAX ? "" : s.substr(minStart, minLen);
}`,
  minwindow_py:`# LC 76: Minimum Window Substring
from collections import Counter

def min_window(s, t):
    need = Counter(t)
    have = {}
    formed = 0
    required = len(need)
    
    left = 0
    min_len = float('inf')
    min_start = 0
    
    for right, c in enumerate(s):
        have[c] = have.get(c, 0) + 1
        
        # Check if current char satisfies need
        if c in need and have[c] == need[c]:
            formed += 1
        
        # Try to shrink window
        while formed == required:
            if right - left + 1 < min_len:
                min_len = right - left + 1
                min_start = left
            
            # Remove leftmost char
            l = s[left]
            left += 1
            have[l] -= 1
            if l in need and have[l] < need[l]:
                formed -= 1
    
    return "" if min_len == float('inf') else s[min_start:min_start+min_len]`,

  longestpal_cpp:`// LC 5: Longest Palindromic Substring
// Key idea: expand from center!
// Every palindrome has a center (odd) or center-gap (even)

string longestPalindrome(string s) {
    int n = s.size();
    int start = 0, maxLen = 1;
    
    auto expand = [&](int l, int r) {
        while (l >= 0 && r < n && s[l] == s[r]) {
            if (r - l + 1 > maxLen) {
                maxLen = r - l + 1;
                start = l;
            }
            l--; r++;
        }
    };
    
    for (int i = 0; i < n; i++) {
        expand(i, i);     // Odd length: "aba"
        expand(i, i+1);   // Even length: "abba"
    }
    
    return s.substr(start, maxLen);
}`,
  longestpal_py:`# LC 5: Longest Palindromic Substring
# Key idea: expand from center!

def longest_palindrome(s):
    n = len(s)
    start, max_len = 0, 1
    
    def expand(l, r):
        nonlocal start, max_len
        while l >= 0 and r < n and s[l] == s[r]:
            if r - l + 1 > max_len:
                max_len = r - l + 1
                start = l
            l -= 1
            r += 1
    
    for i in range(n):
        expand(i, i)      # Odd: "aba" center at i
        expand(i, i+1)    # Even: "abba" center between i,i+1
    
    return s[start:start + max_len]

# "babad" → "bab" or "aba" (both length 3)
# "cbbd" → "bb"`,
};

const LEETCODE = [
  {id:1, num:242, title:"Valid Anagram", diff:"easy", pattern:"Frequency/Hashing", hint:"Count char frequencies in both strings, compare. O(n) time, O(1) space (26 chars)."},
  {id:2, num:49, title:"Group Anagrams", diff:"medium", pattern:"Hashing", hint:"Sort each string as key in hashmap. Or use freq array as key. Group all strings with same key."},
  {id:3, num:3, title:"Longest Substring Without Repeating Characters", diff:"medium", pattern:"Sliding Window", hint:"Sliding window + hashmap. Expand right, shrink left when duplicate found."},
  {id:4, num:76, title:"Minimum Window Substring", diff:"hard", pattern:"Sliding Window", hint:"Two hashmaps (need/have). Expand right to include all chars, shrink left to minimize."},
  {id:5, num:5, title:"Longest Palindromic Substring", diff:"medium", pattern:"Two Pointer / Expand Center", hint:"For each index expand outward checking palindrome. Handle odd & even length."},
  {id:6, num:125, title:"Valid Palindrome", diff:"easy", pattern:"Two Pointer", hint:"Two pointers from both ends. Skip non-alphanumeric. Compare lowercase chars."},
  {id:7, num:151, title:"Reverse Words in a String", diff:"medium", pattern:"Two Pointer / String Manipulation", hint:"Split by spaces, filter empty, reverse list, join. Or do in-place with two pointers."},
  {id:8, num:28, title:"Find the Index of the First Occurrence (strStr)", diff:"easy", pattern:"KMP / Naive", hint:"Use KMP for O(n+m). Build LPS array, then search. Or use built-in find() for interview."},
  {id:9, num:567, title:"Permutation in String", diff:"medium", pattern:"Sliding Window + Frequency", hint:"Fixed window of size len(s1). Maintain freq array. Check if window matches s1 freq."},
  {id:10, num:438, title:"Find All Anagrams in a String", diff:"medium", pattern:"Sliding Window + Frequency", hint:"Same as LC 567 but collect all start indices where match found."},
  {id:11, num:14, title:"Longest Common Prefix", diff:"easy", pattern:"Vertical Scanning", hint:"Compare char by char across all strings. Stop when mismatch or string ends."},
  {id:12, num:394, title:"Decode String", diff:"medium", pattern:"Stack", hint:"Use stack. When '[' push current str and count. When ']' pop and repeat."},
  {id:13, num:647, title:"Palindromic Substrings", diff:"medium", pattern:"Expand Center", hint:"Same as LC 5 expand from center. Count every valid palindrome found."},
  {id:14, num:20, title:"Valid Parentheses", diff:"easy", pattern:"Stack", hint:"Push open brackets, pop on close. Mismatch or non-empty stack = invalid."},
  {id:15, num:459, title:"Repeated Substring Pattern", diff:"easy", pattern:"KMP / String Trick", hint:"Trick: if s is in (s+s)[1:-1], then yes. Or use KMP LPS array."},
  {id:16, num:1143, title:"Longest Common Subsequence", diff:"medium", pattern:"DP on Strings", hint:"2D DP. dp[i][j] = LCS of s1[:i] and s2[:j]. Match: +1, no match: max(dp[i-1][j], dp[i][j-1])."},
  {id:17, num:72, title:"Edit Distance", diff:"hard", pattern:"DP on Strings", hint:"dp[i][j] = min edits to convert s1[:i] to s2[:j]. Three operations: insert, delete, replace."},
  {id:18, num:91, title:"Decode Ways", diff:"medium", pattern:"DP", hint:"dp[i] = ways to decode s[:i]. Single digit valid (1-9), double digit valid (10-26)."},
  {id:19, num:139, title:"Word Break", diff:"medium", pattern:"DP + HashSet", hint:"dp[i] = can s[:i] be segmented. For each i, try all j < i where dp[j] is true and s[j:i] in dict."},
  {id:20, num:8, title:"String to Integer (atoi)", diff:"medium", pattern:"Parsing", hint:"Skip whitespace, handle sign, parse digits, handle overflow with INT_MIN/INT_MAX."},
  {id:21, num:58, title:"Length of Last Word", diff:"easy", pattern:"Traversal", hint:"Traverse from end, skip trailing spaces, count chars until space or start."},
  {id:22, num:271, title:"Encode and Decode Strings", diff:"medium", pattern:"Serialization", hint:'Use length-prefix encoding: "4#word4#test" — store len + "#" + string.'},
  {id:23, num:128, title:"Longest Consecutive Sequence", diff:"medium", pattern:"HashSet", hint:"Put all in set. For each num that is a sequence start (n-1 not in set), count forward."},
  {id:24, num:1047, title:"Remove All Adjacent Duplicates In String", diff:"easy", pattern:"Stack", hint:"Use stack. Push char if top != char, else pop. Join stack for result."},
  {id:25, num:316, title:"Remove Duplicate Letters", diff:"hard", pattern:"Stack + Greedy", hint:"Greedy stack. Track last occurrence. Pop if top > curr and top appears later."},
];

const PRACTICE_50 = [
  {id:1,title:"Check if string is palindrome",diff:"easy",pattern:"Two Pointer"},
  {id:2,title:"Reverse a string",diff:"easy",pattern:"Two Pointer"},
  {id:3,title:"Count vowels in string",diff:"easy",pattern:"Traversal"},
  {id:4,title:"Check anagram",diff:"easy",pattern:"Frequency"},
  {id:5,title:"Find first non-repeating character",diff:"easy",pattern:"Frequency"},
  {id:6,title:"Count occurrences of character",diff:"easy",pattern:"Traversal"},
  {id:7,title:"Remove spaces from string",diff:"easy",pattern:"Traversal"},
  {id:8,title:"Convert to uppercase/lowercase",diff:"easy",pattern:"ASCII"},
  {id:9,title:"Check if two strings are rotations",diff:"easy",pattern:"String Trick"},
  {id:10,title:"Print all characters with frequency",diff:"easy",pattern:"Frequency"},
  {id:11,title:"Find duplicate characters",diff:"easy",pattern:"Frequency"},
  {id:12,title:"Longest palindromic substring",diff:"medium",pattern:"Expand Center"},
  {id:13,title:"Longest substring without repeating",diff:"medium",pattern:"Sliding Window"},
  {id:14,title:"Count palindromic substrings",diff:"medium",pattern:"Expand Center"},
  {id:15,title:"Minimum window substring",diff:"hard",pattern:"Sliding Window"},
  {id:16,title:"Group anagrams together",diff:"medium",pattern:"Hashing"},
  {id:17,title:"Longest common prefix",diff:"easy",pattern:"Vertical Scan"},
  {id:18,title:"String compression (run-length encoding)",diff:"medium",pattern:"Two Pointer"},
  {id:19,title:"Find all permutations of a string",diff:"medium",pattern:"Backtracking"},
  {id:20,title:"Permutation in string (LC 567)",diff:"medium",pattern:"Sliding Window"},
  {id:21,title:"Minimum insertions to make palindrome",diff:"medium",pattern:"DP"},
  {id:22,title:"Longest common subsequence",diff:"medium",pattern:"DP"},
  {id:23,title:"Edit distance",diff:"hard",pattern:"DP"},
  {id:24,title:"Wildcard pattern matching",diff:"hard",pattern:"DP"},
  {id:25,title:"Regular expression matching",diff:"hard",pattern:"DP"},
  {id:26,title:"Implement KMP algorithm",diff:"hard",pattern:"KMP"},
  {id:27,title:"Rabin-Karp pattern search",diff:"hard",pattern:"Rabin-Karp"},
  {id:28,title:"Z-algorithm pattern search",diff:"hard",pattern:"Z-Algo"},
  {id:29,title:"Shortest palindrome (LC 214)",diff:"hard",pattern:"KMP"},
  {id:30,title:"Decode string (LC 394)",diff:"medium",pattern:"Stack"},
  {id:31,title:"Roman to integer",diff:"easy",pattern:"HashMap"},
  {id:32,title:"Integer to Roman",diff:"medium",pattern:"Greedy"},
  {id:33,title:"Zigzag conversion",diff:"medium",pattern:"Simulation"},
  {id:34,title:"Multiply strings",diff:"medium",pattern:"Simulation"},
  {id:35,title:"Valid number",diff:"hard",pattern:"Parsing"},
  {id:36,title:"Word break",diff:"medium",pattern:"DP"},
  {id:37,title:"Word break II",diff:"hard",pattern:"DP + Backtracking"},
  {id:38,title:"Concatenated words",diff:"hard",pattern:"DP + Trie"},
  {id:39,title:"Count distinct subsequences",diff:"hard",pattern:"DP"},
  {id:40,title:"Interleaving string",diff:"hard",pattern:"DP"},
  {id:41,title:"Scramble string",diff:"hard",pattern:"DP"},
  {id:42,title:"Longest duplicate substring",diff:"hard",pattern:"Binary Search + Rabin-Karp"},
  {id:43,title:"Remove duplicate letters (LC 316)",diff:"hard",pattern:"Greedy Stack"},
  {id:44,title:"Largest rectangle from histogram",diff:"hard",pattern:"Stack"},
  {id:45,title:"Minimum # of deletions to make string sorted",diff:"medium",pattern:"DP"},
  {id:46,title:"Count number of homogenous substrings",diff:"medium",pattern:"Math"},
  {id:47,title:"Check if string has all unique characters",diff:"easy",pattern:"Bit Manipulation"},
  {id:48,title:"One Edit Distance",diff:"medium",pattern:"Two Pointer"},
  {id:49,title:"Palindrome Pairs",diff:"hard",pattern:"Trie / HashMap"},
  {id:50,title:"Text Justification",diff:"hard",pattern:"Greedy / Simulation"},
];

// ═══════════════════════════════════ COMPONENTS ═══════════════════════════════════

function StringViz({ str, highlights = {}, label = "" }) {
  return (
    <div style={{margin:"1.5rem 0"}}>
      {label && <p style={{color:"var(--text2)",fontSize:13,marginBottom:8}}>{label}</p>}
      <div style={{display:"flex",gap:6,flexWrap:"wrap"}}>
        {str.split("").map((c, i) => {
          const hl = highlights[i];
          let bg = "var(--bg3)", border = "var(--border)", color = "var(--text)";
          if (hl === "acc") { bg = "rgba(124,58,237,.25)"; border = "#7C3AED"; color = "#A78BFA"; }
          if (hl === "acc2") { bg = "rgba(6,182,212,.25)"; border = "#06B6D4"; color = "#67E8F9"; }
          if (hl === "green") { bg = "rgba(16,185,129,.25)"; border = "#10B981"; color = "#6EE7B7"; }
          if (hl === "warn") { bg = "rgba(245,158,11,.25)"; border = "#F59E0B"; color = "#FCD34D"; }
          if (hl === "danger") { bg = "rgba(239,68,68,.25)"; border = "#EF4444"; color = "#FCA5A5"; }
          return (
            <div key={i} style={{textAlign:"center"}}>
              <div style={{width:40,height:40,background:bg,border:`1.5px solid ${border}`,borderRadius:8,display:"flex",alignItems:"center",justifyContent:"center",color,fontSize:16,fontFamily:"'Fira Code',monospace",fontWeight:500,transition:"all .3s"}}>
                {c}
              </div>
              <div style={{color:"var(--text2)",fontSize:11,marginTop:3}}>{i}</div>
            </div>
          );
        })}
      </div>
    </div>
  );
}

function CodeBlock({ code, lang }) {
  const [copied, setCopied] = useState(false);
  const copy = () => { navigator.clipboard.writeText(code).catch(()=>{}); setCopied(true); setTimeout(()=>setCopied(false),1500); };

  const highlight = (rawCode, language) => {
    // Step 1: Split into lines and process each line to avoid cross-line issues
    const lines = rawCode.split('\n');
    return lines.map(line => {
      // Check if the whole line (trimmed) is a comment — handle first
      const trimmed = line.trimStart();
      const isCppComment = language === 'cpp' && trimmed.startsWith('//');
      const isPyComment = language !== 'cpp' && trimmed.startsWith('#');

      if (isCppComment || isPyComment) {
        // Escape HTML in the comment line and color it green
        const escaped = line.replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;');
        return `<span style="color:#6A9955">${escaped}</span>`;
      }

      // For non-comment lines, escape HTML then apply highlighting
      let hl = line.replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;');

      // For C++, handle inline // comments (everything after //)
      if (language === 'cpp') {
        hl = hl.replace(/(\/\/[^\n]*)$/g, '<span style="color:#6A9955">$1</span>');
      }

      // Strings: double and single quotes
      hl = hl.replace(/("(?:[^"\\]|\\.)*")/g, '<span style="color:#CE9178">$1</span>');
      hl = hl.replace(/('(?:[^'\\]|\\.)*')/g, '<span style="color:#CE9178">$1</span>');

      // Numbers
      hl = hl.replace(/\b(\d+)\b/g, '<span style="color:#B5CEA8">$1</span>');

      // Keywords
      if (language === 'cpp') {
        hl = hl.replace(/\b(int|string|char|bool|void|return|if|else|while|for|auto|using|namespace|include|vector|unordered_map|map|cout|cin|true|false|nullptr|const|class|struct|new|delete|endl)\b/g,
          '<span style="color:#569CD6;font-weight:500">$1</span>');
      } else {
        hl = hl.replace(/\b(def|return|if|elif|else|while|for|in|not|and|or|True|False|None|class|import|from|print|len|range|str|int|list|dict|set|enumerate|Counter|nonlocal|lambda|with|as|pass|break|continue)\b/g,
          '<span style="color:#569CD6;font-weight:500">$1</span>');
      }

      return hl;
    }).join('\n');
  };

  const highlighted = highlight(code, lang);

  return (
    <div style={{background:"var(--cbg)",borderRadius:12,border:"1px solid var(--border)",overflow:"hidden",margin:"1rem 0"}}>
      <div style={{display:"flex",justifyContent:"space-between",alignItems:"center",padding:"8px 16px",background:"rgba(255,255,255,.04)",borderBottom:"1px solid var(--border)"}}>
        <span style={{color:"var(--text2)",fontSize:12}}>{lang==="cpp"?"C++":"Python"}</span>
        <button className="btn" onClick={copy} style={{background:"transparent",color:copied?"#10B981":"var(--text2)",fontSize:12,padding:"2px 8px",borderRadius:6,border:"1px solid var(--border)"}}>
          {copied?"✓ Copied":"Copy"}
        </button>
      </div>
      <pre style={{padding:"16px",overflowX:"auto",fontSize:13,lineHeight:1.7,color:"#D4D4D4"}} dangerouslySetInnerHTML={{__html:highlighted}}/>
    </div>
  );
}

function Quiz({ questions, sectionId, onComplete }) {
  const [answers, setAnswers] = useState({});
  const [submitted, setSubmitted] = useState(false);
  const score = submitted ? questions.filter((q,i) => answers[i] === q.correct).length : 0;
  return (
    <div style={{background:"var(--bg2)",borderRadius:12,border:"1px solid var(--border)",padding:"1.5rem",marginTop:"2rem"}}>
      <h3 className="hd" style={{fontSize:20,color:"var(--acc2)",marginBottom:"1rem"}}>⚡ Quick Quiz</h3>
      {questions.map((q, qi) => (
        <div key={qi} style={{marginBottom:"1.25rem"}}>
          <p style={{fontWeight:500,marginBottom:8}}>{qi+1}. {q.q}</p>
          <div style={{display:"flex",flexDirection:"column",gap:6}}>
            {q.opts.map((opt, oi) => {
              let bg = "var(--bg3)", border = "var(--border)", color = "var(--text)";
              if (submitted) {
                if (oi === q.correct) { bg="rgba(16,185,129,.15)"; border="#10B981"; color="#6EE7B7"; }
                else if (answers[qi] === oi && oi !== q.correct) { bg="rgba(239,68,68,.12)"; border="#EF4444"; color="#FCA5A5"; }
              } else if (answers[qi] === oi) { bg="rgba(124,58,237,.2)"; border="#7C3AED"; }
              return (
                <button key={oi} className="btn" onClick={() => !submitted && setAnswers(a => ({...a,[qi]:oi}))}
                  style={{background:bg,border:`1px solid ${border}`,color,borderRadius:8,padding:"8px 12px",textAlign:"left",fontSize:14,cursor:submitted?"default":"pointer"}}>
                  {String.fromCharCode(65+oi)}. {opt}
                </button>
              );
            })}
          </div>
          {submitted && q.explain && <p style={{fontSize:13,color:"var(--acc3)",marginTop:6,padding:"8px 12px",background:"rgba(16,185,129,.08)",borderRadius:6}}>💡 {q.explain}</p>}
        </div>
      ))}
      {!submitted ? (
        <button className="btn" onClick={() => { setSubmitted(true); if(score===questions.length||Object.keys(answers).length===questions.length) onComplete?.(); }}
          style={{background:"var(--acc)",color:"white",padding:"10px 24px",borderRadius:8,fontWeight:600}}>
          Submit Answers
        </button>
      ) : (
        <div style={{display:"flex",alignItems:"center",gap:12}}>
          <span style={{fontSize:16,fontWeight:600,color:score===questions.length?"#10B981":score>=questions.length/2?"#F59E0B":"#EF4444"}}>
            Score: {score}/{questions.length} {score===questions.length?"🎉":score>=questions.length/2?"👍":"Keep going!"}
          </span>
          <button className="btn" onClick={() => { setAnswers({}); setSubmitted(false); }} style={{background:"var(--bg4)",color:"var(--text2)",padding:"6px 14px",borderRadius:6,fontSize:13}}>Retry</button>
        </div>
      )}
    </div>
  );
}

function SectionCard({ children, style={} }) {
  return <div className="fade" style={{background:"var(--bg2)",borderRadius:16,border:"1px solid var(--border)",padding:"2rem",marginBottom:"1.5rem",...style}}>{children}</div>;
}

function Callout({ type="info", children }) {
  const colors = {info:{bg:"rgba(6,182,212,.1)",border:"#06B6D4",color:"#67E8F9"},warn:{bg:"rgba(245,158,11,.1)",border:"#F59E0B",color:"#FCD34D"},success:{bg:"rgba(16,185,129,.1)",border:"#10B981",color:"#6EE7B7"},danger:{bg:"rgba(239,68,68,.1)",border:"#EF4444",color:"#FCA5A5"}};
  const c = colors[type];
  return <div style={{background:c.bg,borderLeft:`3px solid ${c.border}`,borderRadius:"0 8px 8px 0",padding:"12px 16px",margin:"1rem 0",color:c.color,fontSize:14}}>{children}</div>;
}

function H2({ children }) { return <h2 className="hd" style={{fontSize:26,color:"var(--acc2)",margin:"1.5rem 0 .75rem"}}>{children}</h2>; }
function H3({ children }) { return <h3 style={{fontSize:18,fontWeight:600,color:"var(--text)",margin:"1.25rem 0 .5rem"}}>{children}</h3>; }
function P({ children }) { return <p style={{lineHeight:1.8,color:"var(--text2)",marginBottom:".75rem"}}>{children}</p>; }
function Tag({ label, color }) { const c={purple:"rgba(124,58,237,.2)",cyan:"rgba(6,182,212,.2)",green:"rgba(16,185,129,.2)",amber:"rgba(245,158,11,.2)"}; return <span style={{background:c[color]||c.purple,color:"var(--text)",fontSize:12,padding:"2px 8px",borderRadius:4,marginRight:6}}>{label}</span>; }

// ═══════════════════════════════════ SECTIONS ═══════════════════════════════════

function S0_Welcome({ onLang }) {
  return (
    <div style={{minHeight:"80vh",display:"flex",flexDirection:"column",alignItems:"center",justifyContent:"center",textAlign:"center"}}>
      <div className="fade">
        <div style={{fontSize:64,marginBottom:"1rem"}}>🧵</div>
        <h1 className="hd" style={{fontSize:52,background:"linear-gradient(135deg,#7C3AED,#06B6D4)",WebkitBackgroundClip:"text",WebkitTextFillColor:"transparent",marginBottom:".5rem"}}>
          STRINGS IN DSA
        </h1>
        <p style={{fontSize:18,color:"var(--text2)",maxWidth:480,margin:"0 auto 2.5rem"}}>
          From absolute beginner to FAANG-level. Interactive, visual, and deeply explained.
        </p>
        <div style={{background:"var(--bg2)",border:"1px solid var(--border)",borderRadius:20,padding:"2rem 2.5rem",maxWidth:420,margin:"0 auto"}}>
          <p style={{fontWeight:600,fontSize:16,marginBottom:"1.5rem"}}>👋 Which language do you prefer?</p>
          <div style={{display:"flex",gap:12,justifyContent:"center"}}>
            {["cpp","python"].map(l => (
              <button key={l} className="btn" onClick={() => onLang(l)} style={{flex:1,padding:"1rem",background:"var(--bg3)",border:"2px solid var(--border)",borderRadius:12,color:"var(--text)",fontSize:16,fontWeight:600,cursor:"pointer"}}>
                <div style={{fontSize:32,marginBottom:4}}>{l==="cpp"?"⚙️":"🐍"}</div>
                {l==="cpp"?"C++":"Python"}
              </button>
            ))}
          </div>
          <p style={{color:"var(--text2)",fontSize:12,marginTop:"1rem"}}>All code examples will use your chosen language.</p>
        </div>
      </div>
    </div>
  );
}

function S1_Basics({ lang }) {
  const [animate, setAnimate] = useState(false);
  const word = "HELLO";
  return (
    <div className="fade">
      <h1 className="hd" style={{fontSize:36,marginBottom:"1rem"}}>🔤 What is a String?</h1>
      <SectionCard>
        <H2>The Story of Strings</H2>
        <P>Imagine you have a bunch of letter blocks — like the ones kids play with. Each block has ONE letter. Now, if you <strong style={{color:"var(--acc2)"}}>line them up in a row</strong>, that row is called a <strong style={{color:"var(--acc)"}}>String</strong>.</P>
        <P>That's literally it! A string is just a <em>sequence of characters placed one after another</em>.</P>
        <Callout type="success">🎯 A <strong>Character</strong> = one letter, digit, or symbol. A <strong>String</strong> = many characters in a row.</Callout>
        <StringViz str="HELLO" label='The string "HELLO" — 5 characters, indices 0 to 4' />
        <button className="btn" onClick={() => setAnimate(a=>!a)} style={{background:"var(--acc)",color:"white",padding:"8px 20px",borderRadius:8,marginTop:8}}>
          {animate?"Stop":"Animate"} Characters
        </button>
        {animate && (
          <div style={{display:"flex",gap:6,marginTop:12}}>
            {word.split("").map((c,i) => (
              <div key={i} style={{textAlign:"center"}}>
                <div style={{width:40,height:40,background:"rgba(124,58,237,.25)",border:"1.5px solid #7C3AED",borderRadius:8,display:"flex",alignItems:"center",justifyContent:"center",color:"#A78BFA",fontSize:16,fontWeight:500,animation:`charBounce .6s ${i*0.1}s ease-in-out infinite`}}>{c}</div>
                <div style={{color:"var(--text2)",fontSize:11,marginTop:3}}>{i}</div>
              </div>
            ))}
          </div>
        )}
      </SectionCard>

      <SectionCard>
        <H2>Mutable vs Immutable</H2>
        <P><strong style={{color:"var(--acc)"}}>Immutable</strong> = cannot be changed after creation. <strong style={{color:"var(--acc2)"}}>Mutable</strong> = can be changed.</P>
        <div style={{display:"grid",gridTemplateColumns:"1fr 1fr",gap:12}}>
          <div style={{background:"rgba(239,68,68,.08)",border:"1px solid rgba(239,68,68,.3)",borderRadius:10,padding:16}}>
            <p style={{color:"#FCA5A5",fontWeight:600,marginBottom:6}}>🐍 Python — IMMUTABLE</p>
            <pre className="mono" style={{fontSize:13,color:"var(--text2)"}}>{"s = 'hello'\ns[0] = 'H'  # ERROR!\n# Can't change in place\n# Must create new string"}</pre>
          </div>
          <div style={{background:"rgba(16,185,129,.08)",border:"1px solid rgba(16,185,129,.3)",borderRadius:10,padding:16}}>
            <p style={{color:"#6EE7B7",fontWeight:600,marginBottom:6}}>⚙️ C++ — MUTABLE</p>
            <pre className="mono" style={{fontSize:13,color:"var(--text2)"}}>{'string s = "hello";\ns[0] = \'H\';  // Works!\n// s is now "Hello"'}</pre>
          </div>
        </div>
        <Callout type="warn">⚠️ This is a <strong>common interview trap!</strong> In Python, strings are immutable — you can't change a single character. You must convert to list, change, then join back.</Callout>
      </SectionCard>

      <SectionCard>
        <H2>String Traversal</H2>
        <P>Traversal means <strong style={{color:"var(--acc2)"}}>visiting every character one by one</strong>. Think of reading each letter of a word carefully.</P>
        <CodeBlock code={CODE[`basic_${lang}`]} lang={lang} />
      </SectionCard>

      <SectionCard>
        <H2>Prefix, Suffix & Substring</H2>
        <StringViz str="ABCDE" highlights={{0:"acc",1:"acc",2:"acc"}} label='Prefix "ABC" — starts from index 0' />
        <StringViz str="ABCDE" highlights={{2:"acc2",3:"acc2",4:"acc2"}} label='Suffix "CDE" — ends at last index' />
        <StringViz str="ABCDE" highlights={{1:"green",2:"green",3:"green"}} label='Substring "BCD" — contiguous portion' />
        <H3>Substring vs Subsequence</H3>
        <P><strong style={{color:"var(--acc)"}}>Substring</strong>: contiguous (no gaps). "ACE" is NOT a substring of "ABCDE" but "BCD" is.</P>
        <P><strong style={{color:"var(--acc2)"}}>Subsequence</strong>: can have gaps, but ORDER must be preserved. "ACE" IS a subsequence of "ABCDE".</P>
        <Callout type="info">💡 Memory trick: Sub<strong>string</strong> = string-like = continuous. Sub<strong>sequence</strong> = sequence = order matters but gaps allowed.</Callout>
      </SectionCard>

      <Quiz
        sectionId={1}
        questions={[
          {q:'What is the index of "l" in "Hello"?', opts:["0","1","2","3"], correct:2, explain:'Indexing starts at 0. H=0, e=1, l=2.'},
          {q:"In Python, can you change a character in a string using s[0] = 'X'?", opts:["Yes","No, strings are immutable","Only for short strings","Only with the 'edit' keyword"], correct:1, explain:"Python strings are immutable. You'd need to convert to list first."},
          {q:'Is "ACE" a substring of "ABCDE"?', opts:["Yes, always","No, it has gaps so it\'s a subsequence","Yes, if we sort it","Depends on language"], correct:1, explain:"Substring must be contiguous. ACE has gaps, so it's a subsequence, not a substring."},
        ]}
      />
    </div>
  );
}

function S2_ASCII({ lang }) {
  const [input, setInput] = useState("A");
  const char = input[0] || "A";
  return (
    <div className="fade">
      <h1 className="hd" style={{fontSize:36,marginBottom:"1rem"}}>🔢 ASCII & Unicode</h1>
      <SectionCard>
        <H2>Characters are Numbers in Disguise</H2>
        <P>Computers don't actually know what the letter "A" is. They only understand <strong style={{color:"var(--acc)"}}>numbers</strong>. So smart people created a system called <strong style={{color:"var(--acc2)"}}>ASCII</strong> — a big table that assigns a number to every character.</P>
        <Callout type="success">🎯 ASCII = American Standard Code for Information Interchange. Just a big cheat-sheet: 'A' = 65, 'B' = 66, ... 'a' = 97, 'b' = 98, ... '0' = 48</Callout>
        <div style={{margin:"1.5rem 0"}}>
          <p style={{marginBottom:8,color:"var(--text2)"}}>Try it! Type a character:</p>
          <input value={input} onChange={e => setInput(e.target.value.slice(-1))} maxLength={1}
            style={{background:"var(--bg3)",border:"1.5px solid var(--acc)",borderRadius:8,padding:"8px 16px",color:"var(--text)",fontSize:20,width:60,textAlign:"center",fontFamily:"'Fira Code',monospace"}} />
          <div style={{display:"flex",gap:16,marginTop:16,flexWrap:"wrap"}}>
            {[
              {label:"Character",val:char,color:"var(--acc)"},
              {label:"ASCII Value",val:char.charCodeAt(0),color:"var(--acc2)"},
              {label:"Hex",val:"0x"+char.charCodeAt(0).toString(16).toUpperCase(),color:"var(--acc3)"},
              {label:"Binary",val:char.charCodeAt(0).toString(2).padStart(8,"0"),color:"var(--warn)"},
            ].map(item => (
              <div key={item.label} style={{background:"var(--bg3)",borderRadius:10,padding:"12px 20px",border:"1px solid var(--border)",textAlign:"center"}}>
                <div style={{color:"var(--text2)",fontSize:12,marginBottom:4}}>{item.label}</div>
                <div style={{color:item.color,fontSize:22,fontFamily:"'Fira Code',monospace",fontWeight:600}}>{item.val}</div>
              </div>
            ))}
          </div>
        </div>
        <H3>The Most Important ASCII Values to Memorize</H3>
        <div style={{display:"grid",gridTemplateColumns:"repeat(auto-fit,minmax(150px,1fr))",gap:8,margin:"1rem 0"}}>
          {[["'A'","65"],["'Z'","90"],["'a'","97"],["'z'","122"],["'0'","48"],["'9'","57"],[" ' '","32"],["'\\n'","10"]].map(([c,v]) => (
            <div key={c} style={{background:"var(--bg3)",borderRadius:8,padding:"8px 12px",border:"1px solid var(--border)",display:"flex",justifyContent:"space-between",alignItems:"center"}}>
              <code style={{color:"var(--acc)",fontSize:14}}>{c}</code>
              <span style={{color:"var(--acc2)",fontWeight:600}}>{v}</span>
            </div>
          ))}
        </div>
        <Callout type="warn">🔑 Key Tricks: lowercase - uppercase = 32. So 'a' - 'A' = 97 - 65 = 32. To get index of a letter: c - 'a' gives 0 for a, 1 for b, etc.</Callout>
        <CodeBlock code={CODE[`ascii_${lang}`]} lang={lang} />
      </SectionCard>
      <SectionCard>
        <H2>Unicode — Beyond English</H2>
        <P>ASCII only covers 128 characters (English letters + basic symbols). But what about Hindi, Arabic, Chinese, Emoji? That's where <strong style={{color:"var(--acc)"}}>Unicode</strong> comes in — it covers over 143,000 characters from every language on Earth!</P>
        <Callout type="info">In interviews, ASCII (26 letters) problems use arrays of size 26. Unicode problems use HashMaps since we can't have a huge array.</Callout>
      </SectionCard>
      <Quiz sectionId={2} questions={[
        {q:"What is the ASCII value of 'a'?", opts:["65","97","90","32"], correct:1, explain:"'A' = 65, and lowercase is 32 more, so 'a' = 97."},
        {q:"How do you get the position of a letter (a=0, b=1...) using ASCII?", opts:["c + 'a'","c - 'a'","c * 'a'","c / 26"], correct:1, explain:"'a'-'a'=0, 'b'-'a'=1, etc. This is used constantly in DSA!"},
      ]} />
    </div>
  );
}

function S3_Indexing({ lang }) {
  const [step, setStep] = useState(0);
  const s = "PYTHON";
  const steps = [
    {hl:{0:"acc"},desc:"Index 0: First character 'P'"},
    {hl:{1:"acc"},desc:"Index 1: 'Y'"},
    {hl:{5:"acc"},desc:"Index 5 (last): 'N' — also index -1 in Python"},
    {hl:{0:"acc2",1:"acc2",2:"acc2"},desc:"Slice [0:3] → 'PYT' (indices 0,1,2)"},
    {hl:{2:"green",3:"green",4:"green"},desc:"Slice [2:5] → 'THO'"},
  ];
  return (
    <div className="fade">
      <h1 className="hd" style={{fontSize:36,marginBottom:"1rem"}}>📍 Indexing & Traversal</h1>
      <SectionCard>
        <H2>Think of Positions Like House Numbers</H2>
        <P>Every character in a string has an <strong style={{color:"var(--acc)"}}>address</strong> — we call it an <strong style={{color:"var(--acc2)"}}>index</strong>. The first house is number 0, not 1. (Computer scientists start counting from 0!)</P>
        <StringViz str={s} highlights={steps[step].hl} label={steps[step].desc} />
        <div style={{display:"flex",gap:8,marginTop:8,flexWrap:"wrap"}}>
          {steps.map((st,i) => (
            <button key={i} className="btn" onClick={() => setStep(i)}
              style={{background:step===i?"var(--acc)":"var(--bg3)",color:step===i?"white":"var(--text2)",padding:"6px 14px",borderRadius:8,fontSize:13,border:`1px solid ${step===i?"var(--acc)":"var(--border)"}`}}>
              Step {i+1}
            </button>
          ))}
        </div>
      </SectionCard>
      <SectionCard>
        <H2>Negative Indexing (Python only!)</H2>
        <P>Python lets you use negative indices! -1 is the last character, -2 is second-to-last, etc. This is a Python superpower not available in C++.</P>
        <div style={{display:"flex",gap:6,flexWrap:"wrap",margin:"1rem 0"}}>
          {s.split("").map((c,i) => (
            <div key={i} style={{textAlign:"center"}}>
              <div style={{width:40,height:40,background:"rgba(6,182,212,.2)",border:"1.5px solid #06B6D4",borderRadius:8,display:"flex",alignItems:"center",justifyContent:"center",color:"#67E8F9",fontSize:16,fontFamily:"'Fira Code',monospace",fontWeight:500}}>{c}</div>
              <div style={{color:"#A78BFA",fontSize:10,marginTop:2}}>{i}</div>
              <div style={{color:"#FCD34D",fontSize:10}}>{i-s.length}</div>
            </div>
          ))}
        </div>
        <p style={{fontSize:12,color:"var(--text2)"}}><span style={{color:"#A78BFA"}}>■</span> Positive index &nbsp; <span style={{color:"#FCD34D"}}>■</span> Negative index</p>
      </SectionCard>
      <Quiz sectionId={3} questions={[
        {q:'What does s[2] give for s = "Hello"?', opts:["H","e","l","o"], correct:2, explain:"H=0, e=1, l=2. So s[2] = 'l'."},
        {q:'In Python, what is s[-1] for s = "World"?', opts:["W","o","l","d"], correct:3, explain:"-1 is always the last character."},
      ]} />
    </div>
  );
}

function S4_Substrings() {
  return (
    <div className="fade">
      <h1 className="hd" style={{fontSize:36,marginBottom:"1rem"}}>✂️ Substrings & Subsequences</h1>
      <SectionCard>
        <H2>Substring — No Gaps Allowed</H2>
        <P>A <strong style={{color:"var(--acc)"}}>substring</strong> is a contiguous part of the string. Like cutting out a slice.</P>
        <StringViz str="ABCDEF" highlights={{1:"green",2:"green",3:"green"}} label='"BCD" is a substring of "ABCDEF" — contiguous slice from index 1 to 3' />
        <StringViz str="ABCDEF" highlights={{0:"acc",2:"acc",4:"acc"}} label='"ACE" is NOT a substring — there are gaps between A, C, E' />
      </SectionCard>
      <SectionCard>
        <H2>Subsequence — Order Without Contiguity</H2>
        <P>A <strong style={{color:"var(--acc2)"}}>subsequence</strong> keeps the original order but can skip characters. Think of highlighting certain letters in a book — you skip some, but never go backwards.</P>
        <StringViz str="ABCDEF" highlights={{0:"acc2",2:"acc2",4:"acc2"}} label='"ACE" IS a valid subsequence — we skip B, D but keep order' />
        <Callout type="success">🎯 Quick test: Is "BA" a subsequence of "ABCDEF"? NO! B comes before A in the original, but in "BA" we'd need A before B.</Callout>
        <div style={{overflow:"auto",margin:"1rem 0"}}>
          <table style={{width:"100%",borderCollapse:"collapse",fontSize:14}}>
            <thead>
              <tr style={{background:"var(--bg3)"}}>
                {["Concept","Gaps Allowed?","Order Must Match?","Example"].map(h => <th key={h} style={{padding:"8px 12px",textAlign:"left",color:"var(--text2)",borderBottom:"1px solid var(--border)"}}>{h}</th>)}
              </tr>
            </thead>
            <tbody>
              {[["Substring","❌ No","✅ Yes","BCD in ABCDEF"],["Subsequence","✅ Yes","✅ Yes","ACE in ABCDEF"],["Subset (sets)","✅ Yes","❌ No","Order irrelevant"]].map(r => (
                <tr key={r[0]} style={{borderBottom:"1px solid var(--border)"}}>
                  {r.map((c,i) => <td key={i} style={{padding:"8px 12px",color:i===0?"var(--acc)":"var(--text2)"}}>{c}</td>)}
                </tr>
              ))}
            </tbody>
          </table>
        </div>
      </SectionCard>
      <Quiz sectionId={4} questions={[
        {q:'Is "BC" a substring of "ABCDE"?', opts:["Yes","No"], correct:0, explain:"BC appears at indices 1-2, contiguously. So yes!"},
        {q:'Is "ACD" a subsequence of "ABCDE"?', opts:["Yes","No"], correct:0, explain:"A(0) → C(2) → D(3) — order preserved, gaps OK."},
        {q:'How many substrings does a string of length n have?', opts:["n","n²","n(n+1)/2","2^n"], correct:2, explain:"For each starting index i and ending index j where j>=i, we get one substring. That's n(n+1)/2 total."},
      ]} />
    </div>
  );
}

function S5_Palindrome({ lang }) {
  const [input, setInput] = useState("racecar");
  const isPalin = input === input.split("").reverse().join("");
  return (
    <div className="fade">
      <h1 className="hd" style={{fontSize:36,marginBottom:"1rem"}}>🔄 Palindromes</h1>
      <SectionCard>
        <H2>What's a Palindrome?</H2>
        <P>A palindrome reads the same forwards and backwards. Like "RACECAR" — spell it backward: RACECAR. Same!</P>
        <div style={{margin:"1.5rem 0"}}>
          <p style={{color:"var(--text2)",marginBottom:8}}>Type a word and check:</p>
          <input value={input} onChange={e => setInput(e.target.value.toLowerCase())}
            style={{background:"var(--bg3)",border:`1.5px solid ${isPalin?"#10B981":"var(--border)"}`,borderRadius:8,padding:"8px 16px",color:"var(--text)",fontSize:16,width:"100%",maxWidth:300}} />
          <div style={{marginTop:12,padding:"8px 16px",background:isPalin?"rgba(16,185,129,.1)":"rgba(239,68,68,.1)",border:`1px solid ${isPalin?"#10B981":"#EF4444"}`,borderRadius:8,display:"inline-block",color:isPalin?"#6EE7B7":"#FCA5A5",fontWeight:600}}>
            {isPalin?"✅ Palindrome!":"❌ Not a palindrome"}
          </div>
        </div>
        {input.length > 0 && (
          <>
            <StringViz str={input} label="Forward →" />
            <StringViz str={input.split("").reverse().join("")} label="← Backward" />
          </>
        )}
      </SectionCard>
      <SectionCard>
        <H2>Two Pointer Approach — O(n)</H2>
        <P>Instead of reversing the whole string (which takes extra space), use two pointers. One at the start, one at the end. Move them toward each other, comparing.</P>
        <div style={{position:"relative",overflow:"hidden",background:"var(--bg3)",borderRadius:12,padding:"1.5rem",marginTop:"1rem"}}>
          {["racecar"].map(s => (
            <div key={s}>
              <p style={{color:"var(--text2)",marginBottom:8}}>Checking "{s}"</p>
              <div style={{display:"flex",gap:6,marginBottom:8}}>
                {s.split("").map((c,i) => {
                  const n = s.length;
                  const isPair = (i < Math.floor(n/2));
                  const mirror = n-1-i;
                  return (
                    <div key={i} style={{textAlign:"center"}}>
                      <div style={{width:36,height:36,background: i < Math.floor(n/2) ? "rgba(124,58,237,.25)" : i > Math.floor(n/2) ? "rgba(6,182,212,.25)" : "rgba(245,158,11,.25)", border:`1.5px solid ${i < Math.floor(n/2) ? "#7C3AED" : i > Math.floor(n/2) ? "#06B6D4" : "#F59E0B"}`,borderRadius:8,display:"flex",alignItems:"center",justifyContent:"center",color:"var(--text)",fontSize:15,fontFamily:"'Fira Code',monospace"}}>
                        {c}
                      </div>
                      <div style={{fontSize:10,color:"var(--text2)",marginTop:2}}>{i}</div>
                    </div>
                  );
                })}
              </div>
              <p style={{fontSize:13,color:"#A78BFA"}}>↑ left (violet) vs right (cyan) — they match! → PALINDROME</p>
            </div>
          ))}
        </div>
        <CodeBlock code={CODE[`twoptr_${lang}`]} lang={lang} />
      </SectionCard>
      <Quiz sectionId={5} questions={[
        {q:'Is "abba" a palindrome?', opts:["Yes","No"], correct:0, explain:"a-b-b-a reversed is a-b-b-a. Same!"},
        {q:"What is the time complexity of palindrome check using two pointers?", opts:["O(n²)","O(n log n)","O(n)","O(1)"], correct:2, explain:"We traverse the string once, comparing pairs. O(n) time, O(1) extra space."},
        {q:'What does the two-pointer palindrome check do when s[left] != s[right]?', opts:["Continues anyway","Returns false immediately","Swaps them","Skips to next pair"], correct:1, explain:"One mismatch means it can't be a palindrome — return false immediately!"},
      ]} />
    </div>
  );
}

function S6_Frequency({ lang }) {
  const [word, setWord] = useState("hello");
  const freq = word.toLowerCase().replace(/[^a-z]/g,"").split("").reduce((a,c)=>{a[c]=(a[c]||0)+1;return a},{});
  const sorted = Object.entries(freq).sort((a,b) => b[1]-a[1]);
  const max = sorted[0]?.[1] || 1;
  return (
    <div className="fade">
      <h1 className="hd" style={{fontSize:36,marginBottom:"1rem"}}>📊 Frequency Counting & Hashing</h1>
      <SectionCard>
        <H2>The Frequency Trick — Most Common Pattern!</H2>
        <P>Imagine you have the word "banana". How many times does each letter appear? b=1, a=3, n=2. Counting like this is called <strong style={{color:"var(--acc)"}}>frequency counting</strong>.</P>
        <P>This technique solves <strong style={{color:"var(--acc2)"}}>30%+ of all string interview questions!</strong> Anagrams, most frequent character, first non-repeating character — all use this!</P>
        <div style={{margin:"1.5rem 0"}}>
          <p style={{color:"var(--text2)",marginBottom:8}}>Try it — type any word:</p>
          <input value={word} onChange={e => setWord(e.target.value)}
            style={{background:"var(--bg3)",border:"1.5px solid var(--acc)",borderRadius:8,padding:"8px 16px",color:"var(--text)",fontSize:16,width:"100%",maxWidth:320}} />
          {sorted.length > 0 && (
            <div style={{marginTop:16}}>
              {sorted.map(([c,count]) => (
                <div key={c} style={{display:"flex",alignItems:"center",gap:10,marginBottom:6}}>
                  <span style={{width:24,color:"var(--acc)",fontFamily:"'Fira Code',monospace",fontWeight:600}}>{c}</span>
                  <div style={{flex:1,maxWidth:200,background:"var(--bg3)",borderRadius:4,height:20,overflow:"hidden"}}>
                    <div style={{width:`${(count/max)*100}%`,height:"100%",background:"linear-gradient(90deg,#7C3AED,#06B6D4)",borderRadius:4,transition:"width .3s"}}/>
                  </div>
                  <span style={{color:"var(--text2)",fontSize:13}}>{count}</span>
                </div>
              ))}
            </div>
          )}
        </div>
      </SectionCard>
      <SectionCard>
        <H2>Two Ways to Store Frequency</H2>
        <H3>Method 1: Array of size 26 (faster, only lowercase letters)</H3>
        <StringViz str="hello" highlights={{1:"acc2"}} label='For "hello" — create freq[26], all zeros' />
        <P>For each character c, do: <code style={{color:"var(--acc)"}}>freq[c - 'a']++</code></P>
        <P>h-'a'=7 → freq[7]++, e-'a'=4 → freq[4]++, l-'a'=11 → freq[11]++ (twice!), o-'a'=14 → freq[14]++</P>
        <H3>Method 2: HashMap (any characters, more flexible)</H3>
        <P>Use a dictionary/unordered_map. Key = character, Value = count. Slower than array but handles Unicode, spaces, numbers.</P>
        <CodeBlock code={CODE[`freq_${lang}`]} lang={lang} />
        <Callout type="info">🎯 Interview Signal: If problem mentions "anagram", "duplicate", "frequency", "count characters" → instantly think FREQUENCY MAP!</Callout>
      </SectionCard>
      <Quiz sectionId={6} questions={[
        {q:"Which data structure is faster for counting frequency of 26 lowercase letters?", opts:["HashMap","Array of size 26","LinkedList","Tree"], correct:1, explain:"Array has O(1) access. HashMap has overhead. For fixed alphabet (26 letters), array is fastest."},
        {q:"How do you get the array index for character 'g'?", opts:["'g' - 'a'","'g' + 'a'","ord('g')","ascii('g')"], correct:0, explain:"'g' - 'a' = 103 - 97 = 6. So g maps to index 6."},
        {q:"Two strings are anagrams if...", opts:["They have same length","Their sorted versions match","Their character frequencies are identical","Both A and B"], correct:3, explain:"Same length AND same frequencies (which means sorted versions also match). All three are equivalent checks."},
      ]} />
    </div>
  );
}

function S7_TwoPointer({ lang }) {
  const [tpStep, setTpStep] = useState(0);
  const s = "aabccbaa";
  const steps = [
    {l:0,r:7,msg:"Start: left=0(a), right=7(a) → Match! ✓"},
    {l:1,r:6,msg:"left=1(a), right=6(a) → Match! ✓"},
    {l:2,r:5,msg:"left=2(b), right=5(b) → Match! ✓"},
    {l:3,r:4,msg:"left=3(c), right=4(c) → Match! ✓ left>=right → PALINDROME!"},
  ];
  const cur = steps[tpStep];
  const hlPal = {};
  for(let i=0;i<cur.l;i++) hlPal[i]="green";
  hlPal[cur.l]="acc"; hlPal[cur.r]="acc2";
  return (
    <div className="fade">
      <h1 className="hd" style={{fontSize:36,marginBottom:"1rem"}}>👉👈 Two Pointer Technique</h1>
      <SectionCard>
        <H2>The "Squeeze" Strategy</H2>
        <P>Imagine two people walking toward each other on a path, looking for something. That's the two-pointer technique! Instead of one loop inside another (slow), we use <strong style={{color:"var(--acc)"}}>two pointers</strong> that move smartly.</P>
        <Callout type="success">🎯 Two Pointer always gives O(n) instead of O(n²). It's like going from an hour of work to one minute!</Callout>
        <H3>Visualization — Palindrome Check</H3>
        <StringViz str={s} highlights={hlPal} label={cur.msg} />
        <div style={{display:"flex",gap:8,marginTop:8}}>
          <button className="btn" onClick={() => setTpStep(s=>Math.max(0,s-1))} style={{background:"var(--bg3)",color:"var(--text)",padding:"6px 16px",borderRadius:8,border:"1px solid var(--border)"}}>← Prev</button>
          <button className="btn" onClick={() => setTpStep(s=>Math.min(steps.length-1,s+1))} style={{background:"var(--acc)",color:"white",padding:"6px 16px",borderRadius:8}}>Next →</button>
          <span style={{color:"var(--text2)",fontSize:13,alignSelf:"center"}}>Step {tpStep+1}/{steps.length}</span>
        </div>
      </SectionCard>
      <SectionCard>
        <H2>Two Types of Two Pointers</H2>
        <div style={{display:"grid",gridTemplateColumns:"1fr 1fr",gap:16}}>
          <div style={{background:"rgba(124,58,237,.08)",border:"1px solid rgba(124,58,237,.3)",borderRadius:12,padding:16}}>
            <p style={{color:"#A78BFA",fontWeight:600,marginBottom:8}}>Opposite Direction</p>
            <p style={{color:"var(--text2)",fontSize:14}}>Start from both ends, meet in middle.</p>
            <p style={{color:"var(--text2)",fontSize:13,marginTop:6}}>Use for: Palindrome, Reverse, Two-sum in sorted array</p>
            <pre className="mono" style={{fontSize:12,color:"#A78BFA",marginTop:8}}>{"left=0, right=n-1\nwhile(left < right):\n  ...\n  left++; right--"}</pre>
          </div>
          <div style={{background:"rgba(6,182,212,.08)",border:"1px solid rgba(6,182,212,.3)",borderRadius:12,padding:16}}>
            <p style={{color:"#67E8F9",fontWeight:600,marginBottom:8}}>Same Direction (Fast/Slow)</p>
            <p style={{color:"var(--text2)",fontSize:14}}>Both start from same side, move at different speeds.</p>
            <p style={{color:"var(--text2)",fontSize:13,marginTop:6}}>Use for: Remove duplicates, Sliding window variant</p>
            <pre className="mono" style={{fontSize:12,color:"#67E8F9",marginTop:8}}>{"slow=0, fast=0\nwhile(fast < n):\n  ...\n  fast++\n  slow conditionally"}</pre>
          </div>
        </div>
      </SectionCard>
      <SectionCard>
        <H2>Pattern Recognition — When to Use Two Pointers?</H2>
        {[["Problem says 'palindrome'","Use opposite-direction two pointers"],["Problem says 'reverse'","Use two pointers, swap extremes"],["Sorted array + two values summing to target","Two pointers, move based on sum comparison"],["Remove duplicates in-place","Fast/slow pointer pattern"],].map(([signal,action]) => (
          <div key={signal} style={{display:"flex",gap:12,alignItems:"flex-start",marginBottom:10,padding:"10px 14px",background:"var(--bg3)",borderRadius:8,border:"1px solid var(--border)"}}>
            <span style={{color:"var(--warn)",fontSize:16}}>⚡</span>
            <div><p style={{fontWeight:500,color:"var(--text)"}}>{signal}</p><p style={{color:"var(--text2)",fontSize:13}}>{action}</p></div>
          </div>
        ))}
        <CodeBlock code={CODE[`twoptr_${lang}`]} lang={lang} />
      </SectionCard>
      <Quiz sectionId={7} questions={[
        {q:"Two pointer palindrome check: when do we return false?", opts:["When left > right","When s[left] != s[right]","When we reach the middle","Never"], correct:1, explain:"Any single mismatch means it can't be a palindrome."},
        {q:"Time complexity of two pointer approach vs brute force (nested loops)?", opts:["Same","O(n) vs O(n²)","O(log n) vs O(n)","O(n²) vs O(n³)"], correct:1, explain:"Two pointer is O(n) — one pass. Brute force with two nested loops is O(n²)."},
      ]} />
    </div>
  );
}

function S8_SlidingWindow({ lang }) {
  const [swStep, setSwStep] = useState(0);
  const s = "abcabcbb";
  const windows = [
    {l:0,r:0,hl:{0:"green"},win:"a",msg:"window=[a] len=1"},
    {l:0,r:1,hl:{0:"green",1:"green"},win:"ab",msg:"window=[ab] len=2"},
    {l:0,r:2,hl:{0:"green",1:"green",2:"green"},win:"abc",msg:"window=[abc] len=3 ← MAX so far!"},
    {l:1,r:3,hl:{1:"green",2:"green",3:"acc"},win:"bca",msg:"'a' seen! shrink left to 1. window=[bca] len=3"},
    {l:2,r:4,hl:{2:"green",3:"green",4:"acc"},win:"cab",msg:"'b' seen! shrink left. window=[cab] len=3"},
    {l:3,r:5,hl:{3:"green",4:"green",5:"acc"},win:"abc",msg:"window=[abc] len=3"},
    {l:5,r:6,hl:{5:"green",6:"acc"},win:"cb",msg:"'c' seen! shrink. window=[cb] len=2"},
    {l:6,r:7,hl:{6:"green",7:"acc"},win:"bb",msg:"'b' seen! shrink. Final max=3"},
  ];
  const cur = windows[swStep];
  return (
    <div className="fade">
      <h1 className="hd" style={{fontSize:36,marginBottom:"1rem"}}>🪟 Sliding Window</h1>
      <SectionCard>
        <H2>Think of a Train Window</H2>
        <P>Imagine looking out of a train window. The window shows you part of the scenery. As the train moves, the window slides forward — you lose old scenery on the left and gain new scenery on the right.</P>
        <P>In strings, the <strong style={{color:"var(--acc)"}}>sliding window</strong> is a virtual window that moves over the string. We maintain a <strong style={{color:"var(--acc2)"}}>left and right pointer</strong> defining the window's edges.</P>
        <Callout type="success">🎯 Sliding Window converts O(n²) brute force into O(n) — it's magic!</Callout>
        <H3>Step-by-step: "Longest Substring Without Repeating Characters"</H3>
        <P>For string <code style={{color:"var(--acc)"}}>"abcabcbb"</code>, find longest substring with no repeated characters.</P>
        <StringViz str={s} highlights={cur.hl} label={`Step ${swStep+1}: ${cur.msg}`} />
        <div style={{display:"flex",gap:8,marginTop:8,alignItems:"center",flexWrap:"wrap"}}>
          <button className="btn" onClick={() => setSwStep(s=>Math.max(0,s-1))} style={{background:"var(--bg3)",color:"var(--text)",padding:"6px 16px",borderRadius:8,border:"1px solid var(--border)"}}>← Prev</button>
          <button className="btn" onClick={() => setSwStep(s=>Math.min(windows.length-1,s+1))} style={{background:"var(--acc)",color:"white",padding:"6px 16px",borderRadius:8}}>Next →</button>
          <span style={{color:"#6EE7B7",fontSize:13}}>Window: <strong>[{cur.win}]</strong> | Max found: <strong>3</strong> (abc)</span>
        </div>
      </SectionCard>
      <SectionCard>
        <H2>Fixed vs Variable Window</H2>
        <div style={{display:"grid",gridTemplateColumns:"1fr 1fr",gap:16}}>
          {[["Fixed Window 🔒","Window size k is constant. Slide by 1 each step.","Max sum of k consecutive elements"],["Variable Window 🔓","Window expands when we can, shrinks when we must.","Longest/shortest substring with condition"]].map(([t,d,ex]) => (
            <div key={t} style={{background:"var(--bg3)",borderRadius:12,padding:16,border:"1px solid var(--border)"}}>
              <p style={{fontWeight:600,color:"var(--acc2)",marginBottom:6}}>{t}</p>
              <p style={{color:"var(--text2)",fontSize:14,marginBottom:6}}>{d}</p>
              <p style={{color:"var(--warn)",fontSize:12}}>Example: {ex}</p>
            </div>
          ))}
        </div>
        <H3>The Universal Sliding Window Template</H3>
        <CodeBlock code={CODE[`window_${lang}`]} lang={lang} />
        <Callout type="warn">🚨 Interview Signals → "Substring", "Contiguous", "Longest/Shortest with condition" → SLIDING WINDOW!</Callout>
      </SectionCard>
      <Quiz sectionId={8} questions={[
        {q:"What is the time complexity of sliding window?", opts:["O(n²)","O(n log n)","O(n)","O(1)"], correct:2, explain:"Each element is added and removed at most once. So 2n operations = O(n)."},
        {q:"Which keyword in a problem suggests sliding window?", opts:["'palindrome'","'anagram'","'substring with condition'","'sorted'"], correct:2, explain:"'substring' + some optimization condition = sliding window!"},
        {q:"In variable sliding window, when do you shrink the window?", opts:["Every step","When condition is violated","When left > right","Never"], correct:1, explain:"Shrink only when current window violates the problem's condition."},
      ]} />
    </div>
  );
}

function S9_KMP({ lang }) {
  const [kmpStep, setKmpStep] = useState(0);
  const text = "AABAACAADAABAABA";
  const pattern = "AABA";
  return (
    <div className="fade">
      <h1 className="hd" style={{fontSize:36,marginBottom:"1rem"}}>🔍 Pattern Matching — KMP</h1>
      <SectionCard>
        <H2>Why Naive Search is Slow</H2>
        <P>Imagine finding "AABA" in a long text. Brute force: check every position in text, for each position try matching all of pattern. That's <strong style={{color:"var(--danger)"}}>O(n × m)</strong> which is too slow for long texts.</P>
        <P>KMP (Knuth-Morris-Pratt) is <strong style={{color:"var(--acc3)"}}>O(n + m)</strong> — it's smart about what it already knows!</P>
        <Callout type="success">🎯 KMP Key Idea: When a mismatch occurs, don't start from scratch! Use what you already matched to skip ahead intelligently.</Callout>
      </SectionCard>
      <SectionCard>
        <H2>The LPS Array — KMP's Secret Weapon</H2>
        <P><strong style={{color:"var(--acc)"}}>LPS = Longest Proper Prefix which is also a Suffix</strong></P>
        <P>For each prefix of the pattern, find the longest prefix that is also a suffix. This tells us: "if matching fails here, how far back should we go?"</P>
        <div style={{overflow:"auto",margin:"1rem 0"}}>
          <table style={{borderCollapse:"collapse",fontSize:13}}>
            <thead><tr style={{background:"var(--bg3)"}}>
              {["Pattern","A","A","B","A"].map((h,i) => <th key={i} style={{padding:"6px 14px",border:"1px solid var(--border)",color:i===0?"var(--text2)":"var(--acc)"}}>{h}</th>)}
            </tr></thead>
            <tbody>
              <tr><td style={{padding:"6px 14px",border:"1px solid var(--border)",color:"var(--text2)"}}>Index</td>
                {[0,1,2,3].map(i => <td key={i} style={{padding:"6px 14px",border:"1px solid var(--border)",color:"var(--text2)",textAlign:"center"}}>{i}</td>)}
              </tr>
              <tr><td style={{padding:"6px 14px",border:"1px solid var(--border)",color:"var(--text2)"}}>LPS</td>
                {[0,1,0,1].map((v,i) => <td key={i} style={{padding:"6px 14px",border:"1px solid var(--border)",color:"var(--acc2)",textAlign:"center",fontWeight:600}}>{v}</td>)}
              </tr>
            </tbody>
          </table>
        </div>
        <P>LPS[3]=1 means: if mismatch at index 4, go back to index LPS[3]=1 — we already know the first 1 characters match!</P>
        <CodeBlock code={CODE[`kmp_${lang}`]} lang={lang} />
      </SectionCard>
      <SectionCard>
        <H2>Rabin-Karp — Hash-Based Pattern Matching</H2>
        <P>Instead of comparing character-by-character, <strong style={{color:"var(--acc2)"}}>Rabin-Karp</strong> uses <strong style={{color:"var(--acc)"}}>hashing</strong>. Calculate a hash for the pattern, then slide a window over text calculating hash of each window. Only do character comparison when hashes match!</P>
        <Callout type="info">💡 Average O(n+m), worst case O(nm) if many hash collisions. Great for multiple pattern matching and plagiarism detection!</Callout>
        <H3>Z-Algorithm (Brief Intuition)</H3>
        <P>For each position i, Z[i] = length of longest substring starting at i that matches a prefix of the string. Used for pattern matching similarly to KMP.</P>
      </SectionCard>
      <Quiz sectionId={9} questions={[
        {q:"What is the time complexity of KMP?", opts:["O(nm)","O(n+m)","O(n log m)","O(n²)"], correct:1, explain:"O(n) to search + O(m) to build LPS array = O(n+m). Much better than naive O(nm)!"},
        {q:"KMP is better than brute force because...", opts:["It uses hashing","It never goes backward in the text","It sorts the pattern first","It uses recursion"], correct:1, explain:"KMP never backtracks in the text string. It only backtracks in the pattern using the LPS array."},
      ]} />
    </div>
  );
}

function S10_PatternID() {
  const patterns = [
    {signal:"substring, contiguous, window",algo:"Sliding Window",icon:"🪟",color:"#7C3AED"},
    {signal:"palindrome, mirror, symmetric",algo:"Two Pointer / Expand Center",icon:"👉👈",color:"#06B6D4"},
    {signal:"anagram, permutation, rearrange",algo:"Frequency Map",icon:"📊",color:"#10B981"},
    {signal:"find pattern in text, strStr",algo:"KMP / Rabin-Karp",icon:"🔍",color:"#F59E0B"},
    {signal:"longest/shortest with k distinct",algo:"Sliding Window + HashMap",icon:"🪟📊",color:"#EF4444"},
    {signal:"subsequence, order preserved",algo:"Dynamic Programming (DP)",icon:"📈",color:"#8B5CF6"},
    {signal:"edit distance, transform",algo:"DP on Strings",icon:"🔄",color:"#EC4899"},
    {signal:"prefix, suffix common",algo:"Trie / Z-Algorithm",icon:"🌳",color:"#14B8A6"},
    {signal:"repeated substring, period",algo:"KMP LPS or String Doubling Trick",icon:"🔁",color:"#F97316"},
    {signal:"decode, encode, brackets",algo:"Stack",icon:"📚",color:"#A855F7"},
  ];
  return (
    <div className="fade">
      <h1 className="hd" style={{fontSize:36,marginBottom:"1rem"}}>🧠 Problem Identification Guide</h1>
      <SectionCard>
        <H2>How to Read a Problem Like an Expert</H2>
        <P>When you see a new problem, don't start coding! Follow this 4-step thought process:</P>
        {["1️⃣ READ the problem statement carefully. Extract keywords.","2️⃣ IDENTIFY the pattern using keyword signals below.","3️⃣ THINK of brute force first, then optimize.","4️⃣ CODE the solution step by step."].map(s => (
          <div key={s} style={{padding:"10px 16px",background:"var(--bg3)",borderRadius:8,marginBottom:8,fontSize:15}}>{s}</div>
        ))}
      </SectionCard>
      <SectionCard>
        <H2>Keyword → Pattern Decoder</H2>
        {patterns.map(p => (
          <div key={p.signal} style={{display:"flex",gap:12,padding:"12px 16px",background:"var(--bg3)",borderRadius:10,marginBottom:8,border:"1px solid var(--border)",alignItems:"center"}}>
            <span style={{fontSize:24}}>{p.icon}</span>
            <div style={{flex:1}}>
              <p style={{color:"var(--text2)",fontSize:13,marginBottom:3}}>If you see: <span style={{color:"#FCD34D",fontStyle:"italic"}}>"{p.signal}"</span></p>
              <p style={{fontWeight:600,color:p.color}}>{p.algo}</p>
            </div>
          </div>
        ))}
      </SectionCard>
      <SectionCard>
        <H2>The Optimization Staircase</H2>
        <P>Every good solution goes through these steps. Never skip to the end!</P>
        {[
          ["Step 1","Understand the problem. Write examples.","var(--text2)"],
          ["Step 2","Brute force (nested loops). Get it working first.","#EF4444"],
          ["Step 3","Identify the bottleneck (what's repeated?).","#F59E0B"],
          ["Step 4","Apply the right pattern (sliding window, hashing, etc.).","#10B981"],
          ["Step 5","Optimize space if needed.","#06B6D4"],
          ["Step 6","Test edge cases (empty string, single char, all same chars).","#7C3AED"],
        ].map(([step,desc,color]) => (
          <div key={step} style={{display:"flex",gap:12,marginBottom:10,alignItems:"flex-start"}}>
            <div style={{background:color,borderRadius:6,padding:"2px 8px",color:"white",fontSize:12,fontWeight:600,whiteSpace:"nowrap",marginTop:2}}>{step}</div>
            <p style={{color:"var(--text2)",fontSize:14,lineHeight:1.6}}>{desc}</p>
          </div>
        ))}
      </SectionCard>
      <SectionCard>
        <H2>How Interviewers Think</H2>
        <Callout type="warn">🎯 Interviewers care about <em>your thought process</em> more than the final code. Always think aloud!</Callout>
        {["They first check: Can you understand the problem correctly?","Then: Can you identify the right approach?","Then: Can you write clean, bug-free code?","Then: Do you know time/space complexity?","Finally: Can you handle edge cases?"].map((t,i) => (
          <div key={i} style={{padding:"8px 14px",borderLeft:"3px solid var(--acc)",marginBottom:6,color:"var(--text2)",fontSize:14}}>{t}</div>
        ))}
      </SectionCard>
    </div>
  );
}

function S11_LeetCode({ lang }) {
  const [filter, setFilter] = useState("all");
  const [expanded, setExpanded] = useState(null);
  const filtered = filter==="all" ? LEETCODE : LEETCODE.filter(p => p.diff===filter);
  return (
    <div className="fade">
      <h1 className="hd" style={{fontSize:36,marginBottom:"1rem"}}>💻 LeetCode Top 25 String Problems</h1>
      <div style={{display:"flex",gap:8,marginBottom:"1.5rem",flexWrap:"wrap"}}>
        {["all","easy","medium","hard"].map(f => (
          <button key={f} className="btn" onClick={() => setFilter(f)} style={{background:filter===f?"var(--acc)":"var(--bg2)",color:filter===f?"white":"var(--text2)",padding:"6px 16px",borderRadius:8,border:`1px solid ${filter===f?"var(--acc)":"var(--border)"}`,textTransform:"capitalize"}}>
            {f}
          </button>
        ))}
      </div>
      {filtered.map(p => (
        <div key={p.id} style={{background:"var(--bg2)",border:"1px solid var(--border)",borderRadius:12,marginBottom:10,overflow:"hidden"}}>
          <div onClick={() => setExpanded(expanded===p.id?null:p.id)} style={{display:"flex",justifyContent:"space-between",alignItems:"center",padding:"14px 18px",cursor:"pointer"}}>
            <div style={{display:"flex",alignItems:"center",gap:12}}>
              <span style={{color:"var(--text2)",fontSize:13,minWidth:32}}>#{p.num}</span>
              <span style={{fontWeight:500}}>{p.title}</span>
              <span className={`chip tag-${p.diff[0]}`}>{p.diff}</span>
            </div>
            <div style={{display:"flex",alignItems:"center",gap:8}}>
              <Tag label={p.pattern} color="purple" />
              <span style={{color:"var(--text2)",fontSize:16}}>{expanded===p.id?"▲":"▼"}</span>
            </div>
          </div>
          {expanded===p.id && (
            <div style={{padding:"0 18px 18px",borderTop:"1px solid var(--border)"}}>
              <Callout type="info">💡 {p.hint}</Callout>
              {(p.num === 3 || p.num === 76 || p.num === 5 || p.num === 125 || p.num === 28) && (
                <CodeBlock
                  code={p.num===3 ? CODE[`window_${lang}`] : p.num===76 ? CODE[`minwindow_${lang}`] : p.num===5 ? CODE[`longestpal_${lang}`] : p.num===125 ? CODE[`twoptr_${lang}`] : CODE[`kmp_${lang}`]}
                  lang={lang}
                />
              )}
            </div>
          )}
        </div>
      ))}
    </div>
  );
}

function S12_Practice() {
  const [filter, setFilter] = useState("all");
  const [search, setSearch] = useState("");
  const filtered = PRACTICE_50.filter(p =>
    (filter==="all" || p.diff===filter) &&
    (search==="" || p.title.toLowerCase().includes(search.toLowerCase()) || p.pattern.toLowerCase().includes(search.toLowerCase()))
  );
  return (
    <div className="fade">
      <h1 className="hd" style={{fontSize:36,marginBottom:"1rem"}}>🔥 Practice 50 Problems</h1>
      <div style={{display:"flex",gap:8,marginBottom:12,flexWrap:"wrap"}}>
        {["all","easy","medium","hard"].map(f => (
          <button key={f} className="btn" onClick={() => setFilter(f)} style={{background:filter===f?"var(--acc)":"var(--bg2)",color:filter===f?"white":"var(--text2)",padding:"6px 16px",borderRadius:8,border:`1px solid ${filter===f?"var(--acc)":"var(--border)"}`,textTransform:"capitalize"}}>{f}</button>
        ))}
      </div>
      <input value={search} onChange={e => setSearch(e.target.value)} placeholder="🔎 Search by name or pattern..." style={{background:"var(--bg2)",border:"1px solid var(--border)",borderRadius:8,padding:"8px 14px",color:"var(--text)",fontSize:14,width:"100%",marginBottom:"1rem"}} />
      <div style={{display:"grid",gap:8}}>
        {filtered.map(p => (
          <div key={p.id} style={{display:"flex",alignItems:"center",gap:12,background:"var(--bg2)",border:"1px solid var(--border)",borderRadius:10,padding:"12px 16px"}}>
            <span style={{color:"var(--text2)",fontSize:12,minWidth:24}}>{p.id}</span>
            <span style={{flex:1,fontSize:14}}>{p.title}</span>
            <Tag label={p.pattern} color={p.pattern.includes("Pointer")?"cyan":p.pattern.includes("Window")?"green":p.pattern.includes("DP")?"amber":"purple"} />
            <span className={`chip tag-${p.diff[0]}`}>{p.diff}</span>
          </div>
        ))}
      </div>
      <p style={{color:"var(--text2)",fontSize:13,marginTop:12}}>Showing {filtered.length} of {PRACTICE_50.length} problems</p>
    </div>
  );
}

function S13_Approach() {
  return (
    <div className="fade">
      <h1 className="hd" style={{fontSize:36,marginBottom:"1rem"}}>🚀 How To Solve ANY String Problem</h1>
      <SectionCard>
        <H2>The 7-Question Framework</H2>
        <P>Before touching the keyboard, ask yourself these 7 questions:</P>
        {[
          ["What exactly is the input?","Single string? Two strings? Array of strings?"],
          ["What are the constraints?","Length? Lowercase only? Unicode? Numbers?"],
          ["What keywords do I see?","Palindrome? Substring? Anagram? Pattern?"],
          ["What's the brute force?","Two nested loops? O(n²) or O(n³)?"],
          ["What's being repeated?","What work is done again and again that I can cache?"],
          ["What data structure helps?","HashMap? Array? Stack? Deque?"],
          ["What are the edge cases?","Empty string? Single char? All same chars? All different?"],
        ].map(([q,hint],i) => (
          <div key={i} style={{display:"flex",gap:14,marginBottom:12,padding:"12px 16px",background:"var(--bg3)",borderRadius:10,border:"1px solid var(--border)"}}>
            <div style={{width:28,height:28,borderRadius:"50%",background:"var(--acc)",display:"flex",alignItems:"center",justifyContent:"center",color:"white",fontSize:13,fontWeight:700,flexShrink:0}}>{i+1}</div>
            <div>
              <p style={{fontWeight:600,marginBottom:3}}>{q}</p>
              <p style={{color:"var(--text2)",fontSize:13}}>{hint}</p>
            </div>
          </div>
        ))}
      </SectionCard>
      <SectionCard>
        <H2>Complexity Cheat Table</H2>
        <div style={{overflowX:"auto"}}>
          <table style={{width:"100%",borderCollapse:"collapse",fontSize:13}}>
            <thead><tr style={{background:"var(--bg3)"}}>
              {["Approach","Time","Space","Use When"].map(h=><th key={h} style={{padding:"8px 12px",textAlign:"left",borderBottom:"1px solid var(--border)",color:"var(--text2)"}}>{h}</th>)}
            </tr></thead>
            <tbody>
              {[
                ["Brute Force (nested loops)","O(n²)","O(1)","Rarely — only very small n"],
                ["Two Pointer","O(n)","O(1)","Palindrome, reverse, sorted array"],
                ["Sliding Window","O(n)","O(k)","Substring problems with condition"],
                ["Frequency Array","O(n)","O(1)","26 lowercase letters only"],
                ["HashMap","O(n)","O(n)","Any characters, need mapping"],
                ["KMP / Rabin-Karp","O(n+m)","O(m)","Pattern matching"],
                ["DP","O(n²)","O(n²)","LCS, edit distance, palindrome count"],
                ["Trie","O(n×L)","O(ALPHABET×n)","Prefix queries, word search"],
              ].map(r=>(
                <tr key={r[0]} style={{borderBottom:"1px solid var(--border)"}}>
                  <td style={{padding:"8px 12px",color:"var(--acc)",fontWeight:500}}>{r[0]}</td>
                  <td style={{padding:"8px 12px",color:"#FCA5A5"}}>{r[1]}</td>
                  <td style={{padding:"8px 12px",color:"#FCD34D"}}>{r[2]}</td>
                  <td style={{padding:"8px 12px",color:"var(--text2)"}}>{r[3]}</td>
                </tr>
              ))}
            </tbody>
          </table>
        </div>
      </SectionCard>
      <SectionCard>
        <H2>Common Mistakes to Avoid</H2>
        {[["Off-by-one in substring","Use right-left+1 for length, not right-left"],["Forgetting to reset pointers","Reset left pointer in each sliding window problem"],["Not handling empty string","Always check if(s.empty()) at the start"],["Wrong LPS in KMP","Trace LPS manually before coding it"],["Python string immutability","Convert to list for in-place modifications"],["Overflow in hashing","Use modular arithmetic with a prime mod"],].map(([mistake,fix]) => (
          <div key={mistake} style={{display:"flex",gap:12,marginBottom:8,padding:"10px 14px",background:"rgba(239,68,68,.06)",border:"1px solid rgba(239,68,68,.2)",borderRadius:8}}>
            <span style={{color:"#EF4444"}}>❌</span>
            <div>
              <p style={{fontWeight:500,fontSize:14}}>{mistake}</p>
              <p style={{color:"var(--acc3)",fontSize:13}}>✅ Fix: {fix}</p>
            </div>
          </div>
        ))}
      </SectionCard>
    </div>
  );
}

function S14_Cheatsheet({ lang }) {
  const sections = [
    {title:"Sliding Window Template", code: lang==="cpp" ?
`// Variable Sliding Window
int left = 0, ans = 0;
unordered_map<char,int> window;
for (int right = 0; right < s.size(); right++) {
    window[s[right]]++;  // Expand
    while (/* condition violated */) {
        window[s[left]]--;
        if (window[s[left]] == 0) window.erase(s[left]);
        left++;  // Shrink
    }
    ans = max(ans, right - left + 1);
}` :
`# Variable Sliding Window
left = 0
ans = 0
window = {}
for right, c in enumerate(s):
    window[c] = window.get(c, 0) + 1  # Expand
    while len(window) > 1:  # while condition violated
        window[s[left]] -= 1
        if window[s[left]] == 0:
            del window[s[left]]
        left += 1  # Shrink
    ans = max(ans, right - left + 1)`
    },
    {title:"Two Pointer Template", code: lang==="cpp" ?
`int left = 0, right = s.size() - 1;
while (left < right) {
    if (/* condition */) {
        // process
        left++; right--;
    } else if (/* move left */) {
        left++;
    } else {
        right--;
    }
}` :
`left, right = 0, len(s) - 1
while left < right:
    if s[left] == s[right]:  # condition met
        # process match
        left += 1
        right -= 1
    elif True:  # move left (replace condition)
        left += 1
    else:
        right -= 1`
    },
    {title:"Frequency Count Template", code: lang==="cpp" ?
`// Array method (26 lowercase)
int freq[26] = {0};
for (char c : s) freq[c - 'a']++;

// HashMap method (any chars)
unordered_map<char,int> freq;
for (char c : s) freq[c]++;` :
`# Array method (26 lowercase)
freq = [0] * 26
for c in s:
    freq[ord(c) - ord('a')] += 1

# Counter method (easiest)
from collections import Counter
freq = Counter(s)`
    },
  ];
  return (
    <div className="fade">
      <h1 className="hd" style={{fontSize:36,marginBottom:"1rem"}}>📋 Complete Cheatsheet</h1>
      <SectionCard>
        <H2>Pattern → Algorithm Quick Reference</H2>
        <div style={{display:"grid",gridTemplateColumns:"repeat(auto-fit,minmax(280px,1fr))",gap:10}}>
          {[
            {kw:"substring + condition",algo:"Sliding Window",c:"#7C3AED"},
            {kw:"palindrome",algo:"Two Pointer / Expand Center",c:"#06B6D4"},
            {kw:"anagram / permutation",algo:"Frequency Map",c:"#10B981"},
            {kw:"find pattern in text",algo:"KMP / Rabin-Karp",c:"#F59E0B"},
            {kw:"edit / transform",algo:"Dynamic Programming",c:"#EF4444"},
            {kw:"prefix / common prefix",algo:"Trie / Vertical Scan",c:"#8B5CF6"},
            {kw:"bracket / nested",algo:"Stack",c:"#EC4899"},
            {kw:"repeated substring",algo:"KMP LPS trick",c:"#14B8A6"},
          ].map(item => (
            <div key={item.kw} style={{background:"var(--bg3)",borderRadius:10,padding:"10px 14px",border:`1px solid ${item.c}33`}}>
              <p style={{color:"var(--text2)",fontSize:12,marginBottom:3}}>🔑 "{item.kw}"</p>
              <p style={{color:item.c,fontWeight:600,fontSize:14}}>{item.algo}</p>
            </div>
          ))}
        </div>
      </SectionCard>
      {sections.map((sec) => (
        <SectionCard key={sec.title}>
          <H2>{sec.title}</H2>
          <CodeBlock code={sec.code} lang={lang} />
        </SectionCard>
      ))}
      <SectionCard>
        <H2>ASCII Quick Reference</H2>
        <div style={{display:"grid",gridTemplateColumns:"repeat(auto-fit,minmax(160px,1fr))",gap:8}}>
          {[["'A'-'Z'","65-90"],["'a'-'z'","97-122"],["'0'-'9'","48-57"],["' ' (space)","32"],["'\\n' newline","10"],["lowercase = uppercase + 32",""],["a's index = c - 'a'",""],["uppercase = c & ~32 (bit trick)",""]].map(([k,v]) => (
            <div key={k} style={{background:"var(--bg3)",borderRadius:8,padding:"8px 12px",border:"1px solid var(--border)"}}>
              <code style={{color:"var(--acc)",fontSize:12,display:"block"}}>{k}</code>
              {v && <span style={{color:"var(--acc2)",fontSize:13,fontWeight:600}}>{v}</span>}
            </div>
          ))}
        </div>
      </SectionCard>
      <SectionCard>
        <H2>Interview Tips — Last Minute Revision</H2>
        {["Always clarify: lowercase only? Unicode? Numbers allowed?","State brute force complexity before optimizing","Mention time AND space complexity","Test with: empty string, 1 char, all same chars, all different chars","Think out loud — 50% of marks are for communication","If stuck, try: can I use a hashmap? a two pointer? a window?","For LCS/Edit Distance type: always think 2D DP first"].map((tip,i) => (
          <div key={i} style={{display:"flex",gap:10,marginBottom:8,padding:"8px 12px",background:"var(--bg3)",borderRadius:8,fontSize:14}}>
            <span style={{color:"var(--acc)"}}>→</span>
            <span style={{color:"var(--text2)"}}>{tip}</span>
          </div>
        ))}
      </SectionCard>
    </div>
  );
}

// ═══════════════════════════════════ MAIN APP ═══════════════════════════════════

const SECTION_COMPONENTS = [S0_Welcome,S1_Basics,S2_ASCII,S3_Indexing,S4_Substrings,S5_Palindrome,S6_Frequency,S7_TwoPointer,S8_SlidingWindow,S9_KMP,S10_PatternID,S11_LeetCode,S12_Practice,S13_Approach,S14_Cheatsheet];

export default function StringDSAApp() {
  const [lang, setLang] = useState(null);
  const [theme, setTheme] = useState("dark");
  const [sec, setSec] = useState(0);
  const [done, setDone] = useState(new Set());
  const [sideOpen, setSideOpen] = useState(true);
  const mainRef = useRef(null);

  const goTo = (id) => { setSec(id); mainRef.current?.scrollTo(0,0); };
  const markDone = (id) => setDone(d => new Set([...d, id]));

  const Comp = SECTION_COMPONENTS[sec];
  const progress = Math.round((done.size / (NAV.length-1)) * 100);

  return (
    <div className={theme==="light"?"lt":""} style={{display:"flex",flexDirection:"column",height:"100vh",background:"var(--bg)",color:"var(--text)",overflow:"hidden"}}>
      <style>{STYLES}</style>
      {/* TOP BAR */}
      <div style={{display:"flex",alignItems:"center",gap:12,padding:"0 16px",height:56,background:"var(--bg2)",borderBottom:"1px solid var(--border)",flexShrink:0,zIndex:10}}>
        <button className="btn" onClick={() => setSideOpen(o=>!o)} style={{background:"transparent",color:"var(--text2)",fontSize:18,padding:"4px 8px",borderRadius:6}}>☰</button>
        <span className="hd" style={{fontSize:20,background:"linear-gradient(135deg,#7C3AED,#06B6D4)",WebkitBackgroundClip:"text",WebkitTextFillColor:"transparent"}}>STRINGS DSA</span>
        <div style={{flex:1,maxWidth:200,height:4,background:"var(--border)",borderRadius:2,overflow:"hidden"}}>
          <div style={{height:"100%",width:`${progress}%`,background:"linear-gradient(90deg,#7C3AED,#06B6D4)",borderRadius:2,transition:"width .4s"}}/>
        </div>
        <span style={{color:"var(--text2)",fontSize:12}}>{progress}%</span>
        <div style={{flex:1}}/>
        {lang && <span style={{background:"var(--bg3)",border:"1px solid var(--border)",borderRadius:6,padding:"3px 10px",fontSize:12,color:"var(--acc)"}}>{lang==="cpp"?"C++":"Python"}</span>}
        {lang && <button className="btn" onClick={() => setLang(null)} style={{background:"transparent",color:"var(--text2)",fontSize:12,padding:"3px 8px",borderRadius:6,border:"1px solid var(--border)"}}>Switch</button>}
        <button className="btn" onClick={() => setTheme(t=>t==="dark"?"light":"dark")} style={{background:"var(--bg3)",border:"1px solid var(--border)",borderRadius:6,padding:"4px 10px",fontSize:14,color:"var(--text)"}}>
          {theme==="dark"?"☀️":"🌙"}
        </button>
      </div>
      <div style={{display:"flex",flex:1,overflow:"hidden"}}>
        {/* SIDEBAR */}
        {sideOpen && (
          <div className="sb slide" style={{width:240,background:"var(--bg2)",borderRight:"1px solid var(--border)",overflowY:"auto",flexShrink:0,padding:"8px 0"}}>
            {NAV.map(n => (
              <button key={n.id} className="btn" onClick={() => goTo(n.id)} style={{display:"flex",alignItems:"center",gap:8,width:"100%",padding:"10px 16px",background:sec===n.id?"rgba(124,58,237,.2)":"transparent",borderLeft:sec===n.id?"3px solid #7C3AED":"3px solid transparent",color:sec===n.id?"var(--acc)":"var(--text2)",fontSize:13,fontWeight:sec===n.id?600:400,textAlign:"left",borderRadius:0}}>
                <span style={{fontSize:14}}>{n.icon}</span>
                <span style={{flex:1,lineHeight:1.3}}>{n.label}</span>
                {done.has(n.id) && <span style={{color:"#10B981",fontSize:12}}>✓</span>}
              </button>
            ))}
          </div>
        )}
        {/* MAIN CONTENT */}
        <div ref={mainRef} className="sb" style={{flex:1,overflowY:"auto",padding:"2rem",maxWidth:900}}>
          {!lang && sec===0 ? (
            <S0_Welcome onLang={(l) => { setLang(l); setSec(1); }} />
          ) : !lang ? (
            <div style={{textAlign:"center",padding:"3rem"}}>
              <p style={{color:"var(--text2)",marginBottom:"1rem"}}>Please select a language first.</p>
              <button className="btn" onClick={()=>setSec(0)} style={{background:"var(--acc)",color:"white",padding:"10px 24px",borderRadius:8}}>← Back to Welcome</button>
            </div>
          ) : (
            <Comp lang={lang} onComplete={() => markDone(sec)} />
          )}
          {/* NAVIGATION BUTTONS */}
          {lang && sec > 0 && (
            <div style={{display:"flex",justifyContent:"space-between",marginTop:"2rem",paddingTop:"1.5rem",borderTop:"1px solid var(--border)"}}>
              <button className="btn" onClick={() => goTo(Math.max(1, sec-1))} style={{background:"var(--bg2)",border:"1px solid var(--border)",color:"var(--text2)",padding:"10px 20px",borderRadius:8}}>← Previous</button>
              <div style={{display:"flex",gap:8}}>
                <button className="btn" onClick={() => markDone(sec)} style={{background:"rgba(16,185,129,.15)",border:"1px solid #10B981",color:"#6EE7B7",padding:"10px 16px",borderRadius:8,fontSize:13}}>✓ Mark Done</button>
                {sec < NAV.length-1 && (
                  <button className="btn" onClick={() => { markDone(sec); goTo(sec+1); }} style={{background:"var(--acc)",color:"white",padding:"10px 20px",borderRadius:8}}>Next →</button>
                )}
              </div>
            </div>
          )}
        </div>
      </div>
    </div>
  );
}
