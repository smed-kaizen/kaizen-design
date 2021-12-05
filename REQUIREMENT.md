# What are requirements:
Before developing software, it is very useful to have some initial requirements that can guide you throughout the process
of the design and implementation. Having a clear list of requirements helps you not diverge from the original idea of the app
and potentially wasting a lot of time.

# Functional Requirements:
- The user can add tasks coupled with a difficulty. These costs credit.
- The user cannot add a task if they don't have enough credit for it.
- The user cannot add tasks for future days
- The user cannot change (edit, add or delete) tasks that are in the past (<=yesterday)
- The user can remove present non-done tasks, and they can retrieve the credit back.
- The user can mark the task of today's as done, and the credit spent will be added to their experience.
- The user can edit the title, description and difficulty of the task when there is enough credit.
- Editing a task should refund the credit or spend it when applicable.
- When the user levels up, they have access to more credit and their maximum credit should be increased.
- Not doing any task should take some experience from the user. (To think about more)

# Non-Functional Requirements:
- Privacy: the database should be local, users info should be treated with respect and shouldn't be processed in any way.
- Sync: It is worth to think of a possibility to sync the information of the user between multiple devices: maybe implementing
a server, creating accounts for users and creating an asymmetric key, the server can have access to the public keys and the
private keys that should use a passphrase. This passphrase is only known by the user. (To think about more)
- Application should be fast
- Tasks are re-usable: In order to improve the performance and decrease the size of the database, the database modeling
should take into account that most tasks can be re-used.

