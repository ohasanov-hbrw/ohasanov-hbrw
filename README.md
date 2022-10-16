```cpp
#include <smallBrain.hpp>
//g++ tells me that it could not find "bigBrain.hpp"
#include <examCalendar.hpp>
//automatically updated list of exams
#include <projects.hpp>
//automatically updated list of projects
//#include <luck.hpp>
//ran out of ^ a long time ago

int32_t main(){
  while(brain.alive){ 
    while(exams.empty() && brain.work){
      brain.think(projects[rand() % projects.size()]); 
    }
    while(!exams.empty() && brain.work){ //most of the time
      brain.think(exams[0]); //think the closest exam
    }
    //TODO: FIND ANOTHER THING TO DO
   }
  return 0; //end the loop
}
```
<!---
ohasanov-hbrw/ohasanov-hbrw is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
