This tool, when called by another datasource tool, allows that datasource tool to receive multiple datasets, **along with their metadata** in a single query to an external data source, when the response conforms to the schema below.

## Schema

**JSON schema**:

```
[ {"url":"http://rafalab.jhsph.edu/CGI/model-based-cpg-islands-hg19.txt",
   "name":"Rafa CpG islands (human)",
   "extension":"bed",
   "metadata":{"db_key":"hg19"},
   "extra_data":[{"url":"http://hgdownload.cse.ucsc.edu/goldenpath/hg19/database/refGene.txt.gz",
      "path":"path/to/refGene.txt.gz"}]
  },
  {"url":"http://rafalab.jhsph.edu/CGI/model-based-cpg-islands-ce2.txt",
     "name":"Rafa CpG islands (ce)",
     "extension":"bed",
     "metadata":{"db_key":"ce2"}
  },
  {"url":"http://rafalab.jhsph.edu/CGI/model-based-cpg-islands-mm9.txt",
     "name":"Rafa CpG islands (mouse)",
     "extension":"bed",
     "metadata":{"db_key":"mm9"},
     "extra_data":[{"url":"http://hgdownload.cse.ucsc.edu/goldenpath/mm9/database/refGene.txt.gz",
        "path":"path/to/refGene.txt.gz"}]
  }
]
```

## Toolshed

https://testtoolshed.g2.bx.psu.edu/view/matt-shirley/json_data_source
