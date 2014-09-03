=======
AGI_GeoBig5
=======

## My talk on Going Enterprise with QGIS and PostGIS at AGI GeoBig5 in Belfast, 13th May 2014 ##

Online version available [here](http://archaeogeek.github.io/AGI_GeoBig5)

### Transcript ###

1. Title

2. Talk outline

3. Who are Astun Technology? Astun were founded in 2005 and provide enterprise web-based mapping to (mainly) local authorities, based on the open source geospatial stack

4. Who am I? I'm Jo Cook and I've been working for Astun for 3 years, but with open source geospatial software since 2004

5. What do we mean by the term "Enterprise"?

6. Insert obligatory Star Trek pun here

7. I take the term "Enterprise" to mean extending the software to work within the domain of big systems, with additional security requirements, with a need for auditing, and also potentially complex data workflows.

8. So what does this mean in terms of GIS?

9. It means adding business value, combining your in-house data and workflow with your web-based intra and internet systems, and having a centralised, canonical data store. It also means controlling editing/creation of data, and storing/facilitating metadata for auditing and compliance.

10. Why "Open Source Enterprise"?

11. Open Source solutions tend to have a lower defect density (bugs per 1000 lines of code) and fix time. Scalability and sharing are easier because you're not artifically limited by licensing. Tools now have auditing built in, and we can apply features such as ADFS, IP restriction, VPN access for secure integration within networks.

12. Let's talk about QGIS, which no longer needs any introduction!

13. It's possible to totally customise QGIS for your organisational needs. You can install it silently over a network and control exactly what gets installed, with different options available in different profiles.

14. You can customise the appearance by only loading the relevant toolbars and plugins

15. Other useful options for enterprise use include setting database connections automatically, controlling plugin installation, deploy print templates over a network, change the splashscreen and iconset, and use the new layer definition file to include a reference to both the data and the styling in a shareable manner.

16. PostgreSQL and PostGIS don't need much introduction either! However it's worth pointing out that the later versions (9.2+) are optimised for virtual machines and for multi-processor environments. For example they use less power when idle, and there are huge improvements in the time for scanning large volumes of data. Furthermore you can use GSSAPI for secure authentication.

17. Linking QGIS and PostGIS together, there are things like the new auditor plugin which utilises the postgresql hstore data type and some triggers to provide auditing and roll-back facilities.

18. QGIS forms can be used for validation and restriction of text-based data entry

19. It's easy to imagine a workflow that utilises a dynamic postgresql view showing the results of a postgis st_isvalid() or st_isvalidreasion() function to provide quality control when creating or editing spatial data.

20. So all in all, it's definitely possible to create an entire enterprise GIS solution using these tools (and others)

21. Insert obligatory meerkat "simples" reference, oh too late, I already did

22. Thanks- any questions?


