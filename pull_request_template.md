#### Change
Add `Post` to `NewsStory` base migrator.

#### Purpose
To easily migrate over the client's Bento legacy database to Grove.

#### How to test?

1. Deploy this PR (#1) in KPBS QA env: https://cms.qa.kpbs.psdops.com/_deploy/
2. In KPBS site, change the theme to PR 1:
3. Verify that the following fields are correctly imported.
    1. Title
    2. Published Date
    3. Modified Date
    4. Slug
    5. Desciption
    5. SEO Description
    6. Parent ID
4. Now run a `Post migrator` for the corresponding section(s), then check that it shows up as `Primary Section` or `Secondary Sections` (or both) in the `NewsStory`.

**Check in QA**:

**JIRA Ticket:** https://perfectsense.atlassian.net/browse/KPBS-43
