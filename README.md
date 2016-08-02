# snort_rules
Simple Snort Rule Parser Class

duplicate names (e.g., 'content'keyword) are numbered attributes, where 
the first attribute has no number.  For example, an example rule such as
'alert tcp any any -> any any (msg:"bogus zipper"; content:"bogus"; content:"zipper")
the attribute 'content' would point to "bogus" and 'content2' would point to "zipper"

for use of fast_pattern, set fast_pattern = 1 for just the fast_pattern; for 'only',
use fast_pattern = 'only'; use fast_pattern = '1,20' to use the offset/length modifier
