# CS-106a-Solutions

public void run() {
	GoUp();
	GoRight();
	GoDown();
	GoRighty();
	GoUp();
	GoRight();
	GoDown();
}


private void GoUp() {
		turnLeft();
		while (frontIsClear()) {	
			if (noBeepersPresent()) {
				putBeeper();
			}
				move();
					}		
}
private void GoRight() {
	turnRight();
	for (int i=0; i<4;i++) {
		move();
	}
}
private void GoDown() {
	turnRight();
	while (frontIsClear()) {
		if (noBeepersPresent()) {
			putBeeper();
		}
		move();
	}
}
private void GoRighty() {
	turnLeft();
		for (int i=0; i<4;i++) {
			move();
		}
	}
