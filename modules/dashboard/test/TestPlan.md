# Dashboard Test Plan

1. Log in. Note the time. Log out and log back in after 2 minutes. Check that welcome panel info is correct. 
2. Make sure there is no recruitment target set in the configuration module. Check that an incentive to define a 
  recruitment target is displayed in recruitment panel
3. Put a recruitment target in the configuration module and check that the info in the recruitment panel is correct.
4. Switch to site breakdown and check that info in recruitment panel is correct.
5. Create a candidate and assign it to any site. Inactivate it. Make sure it is NOT taken into account in the gender
   breakdown view (recruitment panel). 
6. Check that site breakdown view (recruitment panel) is correct.
7. Check that scans per site (study progression panel) view is correct (scan dates and scan numbers).
8. Check that recruitment per site view is correct (study progression panel).
9. Verify that for a user with 'Edit imaging browser QC status' permission the My Tasks panel reports the number of new
   scans (i.e. the number of scans on the MRI browser page for which QC status has not been set). Check that site 
   displayed is always 'All'. Click on this task and verify that you go to the MRI Browser page. 
10. Verify that for a user with 'Resolving conflicts' permission the number of data entry conflicts is reported in the 
    My Task panel. If the user also has 'Across all sites access candidates profiles' then the site displayed is 
    'All', otherwise it is set to the site the user belongs to. The number of data entry conflicts is the number of 
    entries in the Unresolved tab of the Conflict Resolver page. Click on this task and check that you go to the 
    Conflict Resolver page.
11. Check that for a user with 'Data Entry' permission, the number of incomplete forms (instruments with Data Entry 
    set to 'In Progress') is displayed in the My Tasks panel. If the user also has 'Across all sites access candidates 
    profiles' then the site displayed is 'All', otherwise it is set to the site the user belongs to and only the 
    candidates that belong to the user's site are considered for the computation of the number of incomplete forms. 
    Clicking on this task should take you to the BVL statistics page, with the stats filtered according to the user's 
    site (or without any filter if the user has 'Across all sites access candidates profiles' permission). 
12. Verify that for a user with 'Can edit final radiological reviews' and 'Can view final radiological reviews' 
    permission, the number of radiological reviews to do is displayed in the My Task panel. Site displayed is always 
    'All'. The number of radiological reviews is the number of entries on the Radiological Review page for which Review 
    Done is not set (i.e. 'No' is chosen in the Selection Filter for the Review Done entry). Clicking on the task should
    take you to that page, with the Selection Filter set correctly.
13. Verify that if a user has 'Across all sites create and edit user accounts' permission, the number of pending 
    account approvals is displayed in the My Task panel. This should be the number of entries in the User Account 
    page with the following Selection Filter: Site set to 'All' and Pending Approval set to 'Yes'. The Site displayed
    will always be 'All'.Check that you are taken to that page (with the Selection Filter correctly set) when you 
    click on the task. 
14. Verify that if a user has 'Across all sites access candidate profiles' permission, the reports works and even
    more important to check without this permission. 
15. Verify that if a user has 'User Management / Survey Participant Management' permission, the number of pending
    account approvals is displayed in the My Task panel. This should be the number of entries in the User Account 
    page with the following Selection Filter: Site set to the user's site and Pending Approval set to 'Yes'. The
    Site displayed will be the user's site. Check that you are taken to that page (with the Selection Filter 
    correctly set) when you click on the task. 
16. Verify that a user with 'Violated Scans: View all-sites Violated Scans' permission has a task with the number
    of violated scans displayed. This is the number of entries on the MRI Violated Scans page. The Site displayed will
    always be 'All'. Check that clicking on the task takes you to the Violated Scans page.
17. Verify that if a user has the 'View and upload files in Document Repository' or 'Delete files in Document Repository'    
    permission, the latest documents to have been edited or uploaded in the document repository are displayed (4 at most)
    in the Document Repository panel. Clicking on a document will display it in the browser. Clicking on the Document
    Repository button takes you to the Document Repository page.
18. Check that if a document notification occurred since the last login, it is labeled as 'New' in the Document 
    Repository panel.
19. Check that a 'New' notification is not labeled 'New' anymore after login in again.
20. Verify that if a user has the 'bvl_feedback' permission, the latest Behavioural Feedback notifications are displayed
    (4 at most) in the Behavioural Feedback panel. Clicking on a feedback thread will take you to the proper page.
21. Check that if a document notification occurred since the last login, it is labeled as 'New' in the Behavioural Feedback panel.
22. Check that a 'New' notification is not labeled 'New' anymore after login in again.
23. Check performance on a large dataset (like IBIS) to make sure the dashboard page displays within a reasonable 
    amount of time.
24. When there are no candidates registered (i.e. first time install), the system should display a message indicating
    that there are no candidates in the DB yet instead of showing the candidates chart.
25. When there are no scans done, the system shoudl display a message indicating that no scans were made instead of 
    showing the scans chart.
