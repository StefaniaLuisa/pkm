
### Team Introductions

- Sydney joined 4Site strategy team (second month)
  - Background: 8.5 years environmental nonprofit digital marketing at Conservation Law Foundation
  - Based in Boston, potentially near colleagues attending NCSL conference
  - Experience: WordPress, Google Analytics, digital marketing campaigns
  - Working with Stef and Brian on strategy projects for FPF
  - Interested in learning about FPF team roles and responsibilities
- Megan leads FPF communications team (2.5 years at FPF)
  - Mountain time zone, Idaho-based (pandemic move from Bay Area)
  - Focus: tech policy communications, privacy
  - Currently managing team with part of staff at NCSL policymaker conference in Boston
  - Adrienne Cuffley out in Greece during meeting
- Joanna: Global communications manager (8 months at FPF)
  - Supports APAC (Asia Pacific), Europe teams and Latin America experts based in US
  - Washington D.C. based
  - Had connection issues joining meeting initially
- Celeste: Intern supporting Megan, Joanna, and Adrienne
  - Georgetown grad student, California native now in D.C.
  - Handles social media and project support tasks
- Heather Schneider: VP of Creative Operations at 4Site
  - D.C. based in Columbia Heights, less than mile walk to office
  - Leads project management team ensuring communication about work queue, deadlines, deliverables

### Site-Wide Search Priority Shift and Technical Discovery

- Stef updated SearchWP Pro plugin with comprehensive custom configuration
  - Created FPF custom search engine indexing categories, tags, issues, publication types, teams, comments
  - Previous default engine severely limited: only searched titles, content, slugs, excerpts, authors
  - Missing all custom attributes that FPF relies on for content organization
  - Original setup appeared to go through multiple hands during website build, losing documentation
- Critical technical issues discovered during Mike knowledge transfer
  - Custom parameter in search causing indexing problems - not default to WordPress search
  - SearchWP Pro license key rejection issue - keeps requiring re-entry each session
  - Cloudflare gateway timeout issues resolved during meeting (external issue, not FPF site)
- Strategic priority change: Site search implementation moved ahead of blog categorization
  - Technical fixes will provide immediate improvement across entire site
  - Blog taxonomy updates won’t take effect until search engine properly configured
  - Estimated 4-5 hours development work for Mike to complete technical implementation

### Advanced Search Configuration Capabilities

- New weighted algorithm with granular control over content prioritization
  - Posts, pages, media types can have different weighting priorities
  - Custom weighting for each post type and taxonomy separately
  - Algorithm accounts for title, content, slug, excerpt weight distribution
- Sophisticated content management features:
  - Pin specific content by ID to top of search results for campaigns
  - Create custom search queries for specific terms (example: “India” returns predetermined priority results)
  - Add synonyms for common misspellings and terminology variations
  - FPF/Future Privacy Forum equivalency built into synonym system
- Rules-based content prioritization options
  - Focus content by post type (posts vs pages priority)
  - Category-specific result ordering
  - Date-based content weighting for campaign management
- Ongoing management requirements - not “set and forget” system
  - Regular optimization based on user feedback and search patterns
  - Quarterly reviews recommended for weighting adjustments
  - Content pinning for active campaigns and cornerstone content

### Comprehensive Blog Categorization Audit Results

- Current state analysis: 2,000+ blog posts with problematic taxonomy structure
  - Most posts tagged with 3-5 tags/issues making content discovery impossible
  - Duplicate taxonomies between “tags” and “issues” creating confusion
  - Heavy over-categorization preventing effective content grouping
- Specific consolidation recommendations:
  - Category cleanup:
    - Merge “Press Releases” and “Press Releases and Statements” (more content under Press Releases)
    - Expand “Filings” to “Policy/Regulatory Filings” for public clarity
    - Eliminate “Uncategorized” category - all content must have proper categorization
    - Address “Global” as child category of “Blog” creating cumbersome URLs
  - Taxonomy restructuring:
    - Combine duplicate “tags” and “issues” into single “Issues” taxonomy
    - Maintain existing cornerstone issues terminology (consistent with rest of FPF site)
    - Add “Region” taxonomy (US, Global, etc.) for geographic content filtering
    - Preserve “Publication Type” with potential addition of press releases
- Proposed new faceted structure for blog filtering:
  - Content Type → Issues → Region → Publication Type → Author → Year
  - Maximum 3 tags per post to maintain broad categorization approach
  - Focus on content groupings rather than granular tagging
  - Search functionality handles specific term discovery

### Content Strategy and Tagging Philosophy

- Fundamental shift from granular to broad categorization approach
  - Tags should group content, not isolate individual pieces
  - Visitors looking for content clusters, not single articles
  - 5-10 pieces minimum content threshold for new categories/tags
  - Search bar handles specific term discovery, facets handle browsing
- Content lifecycle management considerations:
  - Archive older content (5+ years) with proper URL redirection to blog homepage
  - Prioritize manual taxonomy updates for recent posts (last 3-5 years)
  - Deprioritize former staff authors in search weighting rather than removal
  - Remove bylines from archived content while preserving posts
- Future content creation guidelines needed:
  - Adrienne developing team template for content creators
  - Historical approach of “tag everything” counterproductive
  - Need constraints and guidelines for consistent taxonomy application

### Listing Block Technical Resolution

- Fixed long-standing listing block error on global page affecting resource filtering
  - Previous issue: changing resources caused page errors
  - Resolution allows filtering by issue with manual image override capability
  - Created duplicate draft page for safe testing without affecting live site
- Identified ongoing design issue with featured images
  - Current block shows small thumbnails instead of full area coverage
  - Only first featured post gets proper image treatment
  - Recommendation: refactor block for consistent image display across all variations
- Sticky posts functionality restored
  - Can now filter posts without breaking page functionality
  - Automatic content refresh eliminates need for manual content curation
  - Recommendation: remove sticky post requirements for easier content management

### Implementation Timeline and Next Steps

- August 13th, 1pm ET: Mike knowledge transfer and QA session
  - Sydney leading QA testing with FPF communications team
  - Adrienne returning from Greece, available for testing participation
  - Heather has scheduling conflicts but Sydney can proceed independently
  - Alternative: week of August 25th if scheduling conflicts arise
- Blog categorization decision timeline:
  - FPF internal team review of taxonomy recommendations required
  - Adrienne will review meeting recording upon return
  - Team discussion needed on content type bifurcation strategy
  - Manual taxonomy updates for priority content (recent posts)
- Technical development queue:
  - Mike: 4-5 hours search engine implementation (priority #1)
  - ITPI website Hebrew blog display issue (minor request added to queue)
  - SearchWP Pro license key resolution
  - Potential automated script development for bulk taxonomy updates (budget dependent)
- Future optimization planning:
  - Quarterly search performance reviews
  - Content creator training on new taxonomy guidelines
  - Possible early September follow-up if August timeline doesn’t work
  - Long-term consideration: automated historical content taxonomy migration