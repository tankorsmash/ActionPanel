# ActionPanel
small and simple debugging panel for testing out cocos2dx's Actions
It'll work something like this when it's done

![Gif preview](https://giant.gfycat.com/AgonizingWhichAngora.gif)

# Usage
Usage should be something like 

        #include "ActionPanel.h"
        
        auto action_panel = ActionPanel::create();
        scene->addChild(action_panel);
        
        auto some_node_to_animate = scene->getChildByName("some_node_to_animate");
        action_panel->set_target(some_node_to_animate);
        
# Considerations
* I've never shared a Cocos Studio project like that, but if you need to make your own instead of using mine, it's looks a bit like this

![Cocos Studio](http://i.imgur.com/kL2YXlp.png?1)

* The default max slider values for `duration` and `set` are set in the `get_duration` and `get_rate` definitions, if you want to change them. 
* The default targetted X and Y positions are set in the CSB file, targetting the middle of an iPhone screen at a resolution of 960x640
