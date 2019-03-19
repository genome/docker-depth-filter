# docker-depth-filter

Filter a vcf to remove low-depth variant calls

```$ /opt/conda/bin/python3 depth_filter.py -h

usage: depth-filter [-h] [--minimum_depth MINIMUM_DEPTH]
                    [--site-depth-field SITE_DEPTH_FIELD]
                    [--filter-field FILTER_FIELD]
                    input_vcf sample_names output_vcf

positional arguments:
  input_vcf             A VCF file with at least two samples (tumor and
                        normal) and readcount information
  sample_names          comma-separated list of samples to which depth filter
                        will be applied
  output_vcf            Path to write the output VCF file

optional arguments:
  -h, --help            show this help message and exit
  --minimum_depth MINIMUM_DEPTH
                        minimum depth for a variant
  --site-depth-field SITE_DEPTH_FIELD
                        field corresponding to site depth - default DP
  --filter-field FILTER_FIELD
                        if variant doesn't have a given depth, then failing
                        variants will have this string added to their FILTER
                        field```

