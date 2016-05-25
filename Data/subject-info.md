## Subject data
**subject_id** - A unique Zooniverse-assigned identifier for the subject you uploaded. You can access the subject's unique Talk page by appending it to Talk URLS as such:  https://www.zooniverse.org/projects/vrooje/kitteh-zoo/talk/subjects/458025 (for subject 458025).

**project_id** - A unique Zooniverse-assigned project identifier. Note that whereas project ascii names such as Kitteh Zoo or Planet Four can be duplicated across projects, these project_id numbers are unique. All project-specific data in the  Zooniverse database is tracked by this number. You can find the project ID in the top right corner of the project builder above the Project details button in the navigation bar.

**workflow_ids** [array] - Each workflow has a unique ID. This column tells you what workflow(s) *in this project* this given subject is associated with.  For example, [] indicates that this subject is not associated with any workflow;[123] means this subject is associated with workflow 123;  [123, 456] indicates this subject is associated with workflow 123 *and* workflow 456. You can find the workflow ID for by viewing each workflow in the project builder.

**subject_set_id** - Each subject set has a unique ID. Although not obvious from the project builder interface, subjects can belong to multiple subject sets. You can find the subject_set id listed on each subject set page next to the subject set name.

**metadata** {json} - Contains all the information that was present in the manifest file during upload for this subject.

**locations** {json} - Contains the web urls  for all images that make up a single subject so that the images can be downloaded or seen directly by the researcher.

**classifications_by_workflow** {json} - Provides the classification count for each workflow associated with that subject. Format is: {"workflow_id":  number of classifications}. For example {"488":20} means there are 20 classifications already made for this subject in workflow 488

**retired_in_workflow** [array]- Indicates which workflows the subject has been retired in. For example, [] indicates the subject has not yet been retired in any workflow; [123] indicates the subject has been retired in workflow 123; [123, 456] indicates the subject has been retired in both workflow 123 and workflow 456.
