1.Reut Stanislau
2.Email: titoshka@inbox.ru , discord: titoshka #9308
3.Get new knowledge, experience and develop.
4.Swift ,Xcode, GitHub, BitBucket, Foundation, UIKit, CoreData, Real, CoreAnimation, AVFoundation
5.pageControl.numberOfPages = 5
pageControl.radius = 5
pageControl.tintColor = .white
pageControl.currentPageTintColor = textColor
pageControl.padding = 10
pageControl.layer.cornerRadius = 9
pageControl.backgroundColor = IntroBackgtoundOlive

addLabel.font = Rubik16Regular
addLabel.textColor = textColor
addLabel.text = NSLocalizedString(“mood_Add_details”, comment: «")

@objc func handleGesture(gesture: UISwipeGestureRecognizer) -> Void {
    
    isNeedShowHint = false
    
    if gesture.direction == .right {
        print("Swipe Right")
       
        if currentMoodIndex > 0 {
            currentMoodIndex -= 1
            
        }
        pageControl.set(progress: Int(currentMoodIndex), animated: true)

    }
    else if gesture.direction == .left {
        print("Swipe Left")
        if currentMoodIndex < currentMood.maxValue {
            currentMoodIndex += 1
        }
        pageControl.set(progress: Int(currentMoodIndex), animated: true)

       
    }
    else if gesture.direction == .up {
        print("Swipe Up")
    
        
    }
    else if gesture.direction == .left {
        
        print("Swipe Down" )
       
    }
}
6.“iOS Developer” TeachMeSkills
7.A2
