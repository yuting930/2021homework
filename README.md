# 2021homework

week03-2_gult_copy_paste

#include <GL/glut.h>

static void display(void)
{
    glClear(GL_COLOR_BUFFER_BIT | GL_DEPTH_BUFFER_BIT);

    glBegin(GL_TRIANGLES);



                glColor3f(1.0f, 0.0f, 0.0f);   glVertex2f(0.0f,   1.0f);

                glColor3f(0.0f, 1.0f, 0.0f);   glVertex2f(0.87f,  -0.5f);

                glColor3f(0.0f, 0.0f, 1.0f);   glVertex2f(-0.87f, -0.5f);



            glEnd();

    glutSwapBuffers();
}

int main(int argc, char *argv[])
{
    glutInit(&argc, argv);
    glutInitDisplayMode(GLUT_RGB | GLUT_DOUBLE | GLUT_DEPTH);
    glutCreateWindow("GLUT Shapes");

    glutDisplayFunc(display);
    glutMainLoop();
}
------------------------------------------------------------------------------------
week03-3_hand_made

#include <GL/glut.h>

void display()
{
    glClear(GL_COLOR_BUFFER_BIT | GL_DEPTH_BUFFER_BIT);

    glutSolidTeapot(0.3);

    glutSwapBuffers();
}

int main(int argc, char **argv)
{
    glutInit(&argc, argv);
    glutInitDisplayMode(GLUT_RGB | GLUT_DOUBLE | GLUT_DEPTH);
    glutCreateWindow("08160084吳鈺婷");

    glutDisplayFunc(display);
    glutMainLoop();
}
----------------------------------------------------------------------------------
week03-4_argc_argv

#include<stdio.h>
int main(int argc, char**argv)
{
    printf("現在的 argc是:%d\n",argc);
    for(int i=0; i<argc; i++)
    {
        printf("argv[%d]是:%s\n",i,argv[i]);
    }
}
