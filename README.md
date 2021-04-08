1.16.6: Midpoint Karel

public class MidpointKarel extends SuperKarel
{
    public void run()
    {
        midpoint1();
        if(noBallsPresent())
        {
            midpoint5();
            if(noBallsPresent())
            {
                midpoint7();
                if(noBallsPresent())
                {
                    midpoint8();
                    if(noBallsPresent())
                    {
                        midpoint15();
                    }
                }
            }
        }
    }
    private void midpoint1()
    {
        if(frontIsBlocked())
        {
            putBall();
        }
    }
    private void midpoint5()
    {
        for(int i = 0; i < 4; i++)
        {
            move();
        }
        if(frontIsBlocked())
        {
            turnAround();
            for(int i = 0; i < 2; i++)
            {
                move();
            }   
            turnAround();
            putBall();
        }
        else
        {
            turnAround();
            for(int i = 0; i < 4; i++)
            {
                move();
            }
            turnAround();
        }
    }
    private void midpoint7()
    {
        for(int i = 0; i < 6; i++)
        {
            move();
        }
        if(frontIsBlocked())
        {
            turnAround();
            for(int i = 0; i < 3; i++)
            {
                move();
            }
            turnAround();
            putBall();
        }
        else
        {
            turnAround();
            for(int i = 0; i < 6; i++)
            {
                move();
            }
            turnAround();
        }
    }
    private void midpoint8()
    {
        for(int i = 0; i < 7; i++)
        {
            move();
        }
        if(frontIsBlocked())
        {
            turnAround();
            for(int i = 0; i < 4; i++)
            {
                move();
            }
            turnAround();
            putBall();
        }
        else
        {
            turnAround();
            for(int i = 0; i < 7; i++)
            {
                move();
            }
            turnAround();
        }
    }
    private void midpoint15()
    {
        for(int i = 0; i < 14; i++)
        {
            move();
        }
        if(frontIsBlocked())
        {
            turnAround();
            for(int i = 0; i < 7; i++)
            {
                move();
            }
            turnAround();
            putBall();
        }
        else
        {
            turnAround();
            for(int i = 0; i < 14; i++)
            {
                move();
            }
            turnAround();
        }
    }
}

````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````
1.16.5: Double Tennis Balls
public class DoubleTennisBallsKarel extends SuperKarel
{
    public void run()
    {
        move();
        doStuff();
    }
    private void doStuff()
    {
        /**
         * does stuff
         **/
        if(ballsPresent())
        {
            takeBall();
            takeBall();
            takeBall();
            takeBall();
            takeBall();
            takeBall();
            takeBall();
            if(ballsPresent())
            {
                takeBall();
                takeBall();
                takeBall();
                takeBall();
                takeBall();
                takeBall();
                takeBall();
                takeBall();
                takeBall();
                takeBall();
                takeBall();
                takeBall();
                takeBall();
                takeBall();
                if(noBallsPresent())
                {
                    for(int i = 0; i < 42; i++)
                    {
                        putBall();
                    }
                    turnAround();
                    move();
                    turnAround();
                }
            }
            else
            {
                putBall();
                putBall();
                putBall();
                putBall();
                putBall();
                putBall();
                putBall();
                putBall();
                putBall();
                putBall();
                putBall();
                putBall();
                putBall();
                putBall();
                turnLeft();
                turnLeft();
                move();
                turnLeft();
                turnLeft();
            }
        }
        else
        {
            putBall();
            putBall();
            putBall();
            putBall();
            putBall();
            putBall();
            putBall();
            putBall();
            putBall();
            putBall();
            putBall();
            putBall();
            putBall();
            putBall();
            putBall();
            putBall();
            putBall();
            putBall();
            putBall();
            putBall();
            putBall();
            turnLeft();
            turnLeft();
            move();
            turnLeft();
            turnLeft();
        }
    }
    private void dontuse()
    {
        move();
    }
}
